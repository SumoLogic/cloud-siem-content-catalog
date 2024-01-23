# [Rules](README.md): Exposed AWS SNS Topic Created

## Description
An AWS Simple Notification Service (SNS ) topic was created allowing all users access to perform actions against the created topic

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Collection|
|Apply Risk to Entities|user_username|
|Signal Name|Exposed AWS SNS Topic Created|
|Summary Expression|{{user_username}} has created an SNS topic that allows all users access|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0009, _mitreAttackTechnique:T1530|
## Vendors and Products
- [Amazon AWS - CloudTrail](../products/033624b0-218e-4dcb-b93f-0f1fb1806c56.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|action|
|Normalized Schema|application|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|user_username|


