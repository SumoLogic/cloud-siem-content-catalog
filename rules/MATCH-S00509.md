# [Rules](README.md): Logon with Local Credentials

## Description
Observes for unexpected local logins. This rule includes 2 match lists to be populated with the active directory domains and permitted local accounts.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Credential Access|
|Apply Risk to Entities|user_username|
|Signal Name|Logon with Local Credentials|
|Summary Expression|Local logon from user: {{user_username}} on host: {{device_hostname}}|
|Score/Severity|Static: 1|
|Enabled by Default|False|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0001, _mitreAttackTactic:TA0003, _mitreAttackTactic:TA0004, _mitreAttackTactic:TA0005, _mitreAttackTactic:TA0006, _mitreAttackTechnique:T1078, _mitreAttackTechnique:T1078.003|
## Vendors and Products
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|device_hostname|
|Normalized Schema|errorCode|
|Normalized Schema|listMatches|
|Normalized Schema|logonType|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|user_authDomain|
|Normalized Schema|user_username|


