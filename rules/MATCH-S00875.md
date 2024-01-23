# [Rules](README.md): AWS VPC FLow Log Deletion

## Description
Detects when a VPC Flow log is deleted which should be an indicator of defense evasion and removal of compromise traces.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Defense Evasion|
|Apply Risk to Entities|user_username|
|Signal Name|AWS VPC FLow Log Deletion|
|Summary Expression|AWS VPC Flow log was deleted by {{user_username}}|
|Score/Severity|Static: 2|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0005, _mitreAttackTechnique:T1070|
## Vendors and Products
- [Amazon AWS - CloudTrail](../products/033624b0-218e-4dcb-b93f-0f1fb1806c56.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|user_username|


