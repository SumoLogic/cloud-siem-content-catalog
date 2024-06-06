# [Rules](README.md): Mimikatz via Powershell and EventID 4703

## Description
Observes for eventID 4703 with SeDebugPrivileges added by powershell. May indicate the presence of Mimikatz credential dumping.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Credential Access|
|Apply Risk to Entities|device_hostname, device_ip, user_username|
|Signal Name|Mimikatz via Powershell and EventID 4703|
|Summary Expression|Potential Mimikatz credential dumping activity on host: {{device_hostname}}|
|Score/Severity|Static: 4|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0006, _mitreAttackTactic:TA0005, _mitreAttackTactic:TA0008, _mitreAttackTechnique:T1555, _mitreAttackTechnique:T1547, _mitreAttackTechnique:T1547.005, _mitreAttackTechnique:T1555.003, _mitreAttackTechnique:T1555.004, _mitreAttackTechnique:T1134, _mitreAttackTechnique:T1134.005, _mitreAttackTechnique:T1098, _mitreAttackTechnique:T1003, _mitreAttackTechnique:T1003.001, _mitreAttackTechnique:T1003.002, _mitreAttackTechnique:T1003.004, _mitreAttackTechnique:T1207, _mitreAttackTechnique:T1558, _mitreAttackTechnique:T1558.001, _mitreAttackTechnique:T1558.002, _mitreAttackTechnique:T1552, _mitreAttackTechnique:T1552.004, _mitreAttackTechnique:T1550, _mitreAttackTechnique:T1550.002, _mitreAttackTechnique:T1550.003|
## Vendors and Products
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|baseImage|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Direct from Record|fields['EventData.EnabledPrivilegeList']|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|user_username|


