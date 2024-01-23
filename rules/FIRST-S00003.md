# [Rules](README.md): First Seen AWS Secrets Manager API Call from User

## Description
Observes for a user performing a ListSecrets API call for the first time.

## Additional Details
|Detail|Value|
|----|----|
|Type|First Seen|
|Category|Collection|
|Apply Risk to Entities|user_username|
|Signal Name|First Seen AWS Secrets Manager API Call from User|
|Summary Expression|User: {{user_username}} observed executing API Call: {{action}} for service: {{application}}|
|Retention Window|7776000000|
|Baseline Window|2592000000|
|Baseline Type|GLOBAL|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0009, _mitreAttackTactic:TA0006, _mitreAttackTechnique:T1552, _mitreAttackTechnique:T1552.004, _mitreAttackTechnique:T1552.005|
## Vendors and Products
- [Amazon AWS - CloudTrail](../products/033624b0-218e-4dcb-b93f-0f1fb1806c56.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|action|
|Normalized Schema|application|
|Direct from Record|fields["userIdentity.type"]|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|user_username|
|Normalized Schema|user_username_role|


