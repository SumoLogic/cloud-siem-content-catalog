# [Rules](README.md): AWS Secrets Manager Enumeration

## Description
A ListSecrets API call has been made to the AWS Secrets Manager service. Ensure that this activity is expected and authorized.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Credential Access|
|Apply Risk to Entities|user_username|
|Signal Name|AWS Secrets Manager Enumeration|
|Summary Expression|{{user_username}} has enumerated AWS Secrets Manager secrets|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0006, _mitreAttackTechnique:T1552, _mitreAttackTactic:TA0007, _mitreAttackTechnique:T1580|
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


