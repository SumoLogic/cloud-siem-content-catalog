# [Rules](README.md): First Seen DynamoDB Enumeration from User

## Description
A user was observed as performing enumeration of DynamoDB tables for the first time in the baseline period.

## Additional Details
|Detail|Value|
|----|----|
|Type|First Seen|
|Category|Collection|
|Apply Risk to Entities|user_username|
|Signal Name|First Seen DynamoDB Enumeration from User|
|Summary Expression|User: {{user_username}} observed enumerating DynamoDB service: {{application}} with the call: {{action}}|
|Retention Window|7776000000|
|Baseline Window|3024000000|
|Baseline Type|GLOBAL|
|Score/Severity|Static: 2|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0009, _mitreAttackTactic:TA0007, _mitreAttackTechnique:T1530, _mitreAttackTechnique:T1526|
## Vendors and Products
- [Amazon AWS - CloudTrail](../products/033624b0-218e-4dcb-b93f-0f1fb1806c56.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|action|
|Normalized Schema|application|
|Direct from Record|fields["userIdentity.type"]|
|Normalized Schema|lower|
|Normalized Schema|metadata_product|
|Normalized Schema|user_username|
|Normalized Schema|user_username_role|


