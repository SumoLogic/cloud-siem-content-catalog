# [Rules](README.md): AWS DynamoDB Outlier in GetItem Events from User

## Description
An outlier in GetItem events to a DynamoDB resource within an hour time period has been detected. Ensure that the user performing these actions has business justification for modifying DynamoDB tables and instances. Consider excluding authorized users from this signal or tweaking the minimum count value if this signal is triggering too often. Data events from DynamoDB are required in order for this signal to function.

## Additional Details
|Detail|Value|
|----|----|
|Type|Outlier|
|Category|Impact|
|Apply Risk to Entities|user_username|
|Signal Name|Spike in DynamoDB GetItem events from User: {{user_username}}|
|Summary Expression|An outlier in PutItem events from a user: {{user_username}}  within an hour time period has been detected|
|Retention Window|7776000000|
|Baseline Window|2592000000|
|Standard Deviation Threshold|1|
|Floor Value|5|
|Score/Severity|Static: 1|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0040, _mitreAttackTechnique:T1565.001|
## Vendors and Products
- [Amazon AWS - CloudTrail](../products/033624b0-218e-4dcb-b93f-0f1fb1806c56.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|action|
|Normalized Schema|application|
|Direct from Record|fields["eventCategory"]|
|Normalized Schema|metadata_vendor|
|Normalized Schema|user_username|


