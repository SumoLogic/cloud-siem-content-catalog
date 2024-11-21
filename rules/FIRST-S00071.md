# [Rules](README.md): First Seen AWS ConsoleLogin by User

## Description
First observance of a user logging on to the Amazon AWS console. This could be indicative of new administrator onboarding, or an unauthorized access to the AWS console. Recommended to investigate the nature of the user account and the login.

## Additional Details
|Detail|Value|
|----|----|
|Type|First Seen|
|Category|Discovery|
|Apply Risk to Entities|user_username|
|Signal Name|First Seen AWS ConsoleLogin by User: {{user_username}}|
|Summary Expression|First Seen AWS ConsoleLogin by {{user_username}}|
|Retention Window|7776000000|
|Baseline Window|2592000000|
|Baseline Type|GLOBAL|
|Score/Severity|Static: 1|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0007, _mitreAttackTechnique:T1538|
## Vendors and Products
- [Amazon AWS - CloudTrail](../products/033624b0-218e-4dcb-b93f-0f1fb1806c56.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|action|
|Normalized Schema|metadata_vendor|
|Normalized Schema|objectType|
|Normalized Schema|success|
|Normalized Schema|user_username|


