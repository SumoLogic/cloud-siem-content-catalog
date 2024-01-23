# [Rules](README.md): Spike in AWS API Call from User

## Description
This rule is designed to detect spikes of excessive API call events within AWS performed by a user based on a daily outliers standard deviation using a designated historic baseline. The minimum floor of API Calls expected by default is set to 5. If excessive signaling is observed it is recommended adding expected users that are known to be involved with specific administrative or privileged activity in AWS to the AWS_admin_users match list.

## Additional Details
|Detail|Value|
|----|----|
|Type|Outlier|
|Category|Execution|
|Apply Risk to Entities|user_username|
|Signal Name|Spike in AWS API Call from User|
|Summary Expression|Excessive count of AWS API Call from User: {{user_username}} based on daily historic activity|
|Retention Window|7776000000|
|Baseline Window|1296000000|
|Standard Deviation Threshold|1|
|Floor Value|5|
|Score/Severity|Static: 2|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0002|
## Vendors and Products
- [Amazon AWS - CloudTrail](../products/033624b0-218e-4dcb-b93f-0f1fb1806c56.md)


## Fields Used

|Origin|Field|
|----|----|
|Direct from Record|fields["userIdentity.type"]|
|Normalized Schema|isEmpty|
|Normalized Schema|listMatches|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|user_username|
|Normalized Schema|user_username_role|


