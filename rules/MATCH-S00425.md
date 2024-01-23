# [Rules](README.md): PowerShell Rundll32 Remote Thread Creation

## Description
Detects PowerShell remote thread creation in Rundll32.exe.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Defense Evasion|
|Apply Risk to Entities|device_hostname, device_ip, user_username|
|Signal Name|PowerShell Rundll32 Remote Thread Creation|
|Summary Expression|Sysmon observed action: {{action}} performed on host: {{device_hostname}}|
|Score/Severity|Static: 4|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0005, _mitreAttackTactic:TA0008, _mitreAttackTechnique:T1021, _mitreAttackTechnique:T1218, _mitreAttackTechnique:T1218.011, _mitreAttackTechnique:T1021.006, _mitreAttackTechnique:T1059, _mitreAttackTechnique:T1059.001, _mitreAttackTechnique:T1059.003|
## Vendors and Products
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|baseImage|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|file_path|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|user_username|


