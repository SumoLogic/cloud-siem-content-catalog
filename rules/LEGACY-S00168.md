# [Rules](README.md): Windows Account Locked Out - 4740

## Description
This signal fires whenever Windows Event type 4740 is seen in the environment.

## Additional Details
|Detail|Value|
|----|----|
|Type|Match|
|Category|Credential Access|
|Apply Risk to Entities|device_hostname, device_ip, user_username, srcDevice_hostname|
|Signal Name|Windows Account Locked Out - 4740|
|Summary Expression|User: {{user_username}} locked out|
|Score/Severity|Static: 2|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0001, _mitreAttackTactic:TA0003, _mitreAttackTactic:TA0004, _mitreAttackTactic:TA0005, _mitreAttackTactic:TA0006, _mitreAttackTactic:TA0040, _mitreAttackTechnique:T1078, _mitreAttackTechnique:T1078.001, _mitreAttackTechnique:T1078.002, _mitreAttackTechnique:T1078.003, _mitreAttackTechnique:T1110, _mitreAttackTechnique:T1110.001, _mitreAttackTechnique:T1110.002, _mitreAttackTechnique:T1110.003, _mitreAttackTechnique:T1110.004, _mitreAttackTechnique:T1531|
## Vendors and Products
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|srcDevice_hostname|
|Normalized Schema|user_username|


