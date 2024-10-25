# [Rules](README.md): AWS Bedrock Guardrail Deleted

## Description
AWS Bedrock Guardrails provide users with the ability to configure options like filtering out harmful content or defining denied topics for models. Guardrails also allow the blocking of sensitive information such as PII. Ensure that this deletion was performed by an authorized user during an expected change. Look at other activity from this user account, focusing on the Bedrock service and pivoting from there if the event is deemed suspicious.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Defense Evasion|
|Apply Risk to Entities|user_username|
|Signal Name|AWS Bedrock Guardrail Deleted|
|Summary Expression|AWS Bedrock Guardrail Deleted by {{user_username}}|
|Score/Severity|Static: 1|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0005, _mitreAttackTechnique:T1562|
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


