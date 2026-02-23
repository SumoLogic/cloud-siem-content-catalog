# [Rules](README.md): First Seen AWS SSM activity by User

## Description
This is the first observance of an account’s activity in the Amazon AWS System Manager Session Manager (SSM). This could be indicative of administrative activity or unauthorized access to the AWS EC2 instance management interface. It is recommended to investigate the account and activity to ensure it is authorized.

## Additional Details
|Detail|Value|
|----|----|
|Type|First Seen|
|Category|Discovery|
|Apply Risk to Entities|user_username|
|Signal Name|First Seen AWS SSM activity by User: {{user_username}}|
|Summary Expression|First Seen AWS ConsoleLogin by {{user_username}}  performing {{action}}|
|Retention Window|7776000000|
|Baseline Window|2592000000|
|Baseline Type|GLOBAL|
|Score/Severity|Static: 2|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0007, _mitreAttackTechnique:T1538|
## Vendors and Products
- [Amazon AWS - CloudTrail](../products/033624b0-218e-4dcb-b93f-0f1fb1806c56.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|user_username|
|Normalized Schema|user_username_role|


