# [Rules](README.md): AWS DynamoDB Outlier in PutItem Events from User

## Description
[Disabled by Default] This rule detects an unusual amount of PutItem events to a DynamoDB resource within an hour time period (DynamoDB data events are required). Verify the user is authorized to modify the DynamoDB tables and instances. This rule is disabled by default due to potential volume of signals, before enabling consider excluding authorized users via match lists, and adjust floor value and model sensitivity as needed.

## Additional Details
|Detail|Value|
|----|----|
|Type|Outlier|
|Category|Impact|
|Apply Risk to Entities|user_username|
|Signal Name|Spike in DynamoDB PutItem Events from User: {{user_username}}|
|Summary Expression|An outlier in PutItem events from a user: {{user_username}}  within an hour time period has been detected|
|Retention Window|7776000000|
|Baseline Window|2592000000|
|Standard Deviation Threshold|1|
|Floor Value|5|
|Score/Severity|Static: 1|
|Enabled by Default|False|
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


