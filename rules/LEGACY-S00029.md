# [Rules](README.md): Disabled Account Logon Attempt

## Description
Detects a disabled account being used for a logon attempt in a Windows environment.

## Additional Details
|Detail|Value|
|----|----|
|Type|Match|
|Category|Credential Access|
|Apply Risk to Entities|srcDevice_ip, user_username, srcDevice_hostname|
|Signal Name|Disabled Account Logon Attempt|
|Summary Expression|Disabled user: {{user_username}} attempted to logon|
|Score/Severity|Static: 6|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0001, _mitreAttackTactic:TA0003, _mitreAttackTactic:TA0004, _mitreAttackTactic:TA0005, _mitreAttackTactic:TA0006, _mitreAttackTechnique:T1078, _mitreAttackTechnique:T1078.001, _mitreAttackTechnique:T1078.002, _mitreAttackTechnique:T1078.003, _mitreAttackTechnique:T1110, _mitreAttackTechnique:T1110.001, _mitreAttackTechnique:T1110.002, _mitreAttackTechnique:T1110.003, _mitreAttackTechnique:T1110.004|
## Vendors and Products
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|action|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_vendor|
|Normalized Schema|srcDevice_hostname|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|user_username|


