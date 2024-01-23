# [Rules](README.md): Spike in AWS AccessDenied Events by assumedrole

## Description
Assuming a role involves using a set of temporary security credentials that can be used to access AWS resources that a role might not normally have access to.

## Additional Details
|Detail|Value|
|----|----|
|Type|Outlier|
|Category|Credential Access|
|Apply Risk to Entities|user_username|
|Signal Name|Spike in AWS AccessDenied Events by assumedrole|
|Summary Expression|Spike in AWS AccessDenied Events by assumedrole {{user_username}}|
|Retention Window|7776000000|
|Baseline Window|1296000000|
|Standard Deviation Threshold|1|
|Floor Value|1|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0006|
## Vendors and Products
- [Amazon AWS - CloudTrail](../products/033624b0-218e-4dcb-b93f-0f1fb1806c56.md)


## Fields Used

|Origin|Field|
|----|----|
|Direct from Record|fields["errorCode"]|
|Direct from Record|fields["userIdentity.type"]|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|user_username|


