# [Rules](README.md): First Seen AWS Bedrock API Call from User

## Description
This rule looks for a first seen AWS Bedrock API call from a user since the baseline period. Ensure the user in question is authorized to utilize AWS Bedrock services. Take a look at the "action" field to determine what API calls are being made and whether this activity is expected.

## Additional Details
|Detail|Value|
|----|----|
|Type|First Seen|
|Category|Discovery|
|Apply Risk to Entities|user_username|
|Signal Name|First Seen AWS Bedrock API Call ({{action}})  from User|
|Summary Expression|The user {{user_username}} has performed an operation within AWS Bedrock: {{action}}  for the first time since the baseline period.|
|Retention Window|3456000000|
|Baseline Window|3024000000|
|Baseline Type|PER_ENTITY|
|Score/Severity|Static: 1|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0007, _mitreAttackTechnique:T1580|
## Vendors and Products
- [Amazon AWS - CloudTrail](../products/033624b0-218e-4dcb-b93f-0f1fb1806c56.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|action|
|Normalized Schema|application|
|Normalized Schema|cloud_provider|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|user_username|


