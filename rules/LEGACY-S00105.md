# [Rules](README.md): Suspicious DC Logon

## Description
Shows RemoteInteractive logons, such as RDP sessions, to domain controllers. Requires customer to setup the domain_controller_hostnames match list

## Additional Details
|Detail|Value|
|----|----|
|Type|Match|
|Category|Lateral Movement|
|Apply Risk to Entities|srcDevice_ip, dstDevice_hostname, user_username|
|Signal Name|Suspicious DC Logon|
|Summary Expression|Suspicious logon to domain controller {{device_hostname}}|
|Score/Severity|Static: 2|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0001, _mitreAttackTactic:TA0003, _mitreAttackTactic:TA0004, _mitreAttackTactic:TA0005, _mitreAttackTactic:TA0008, _mitreAttackTechnique:T1021, _mitreAttackTechnique:T1021.001, _mitreAttackTechnique:T1021.006, _mitreAttackTechnique:T1078, _mitreAttackTechnique:T1078.001, _mitreAttackTechnique:T1078.002, _mitreAttackTechnique:T1078.003|
## Vendors and Products
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|dstDevice_hostname|
|Normalized Schema|listMatches|
|Normalized Schema|logonType|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|user_username|


