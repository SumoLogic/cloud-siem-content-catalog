# [Rules](README.md): Suspicious Writes To Windows Recycle Bin

## Description
This rule detects writes to the recycle bin by a process other than explorer.exe.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Collection|
|Apply Risk to Entities|device_hostname, device_ip, user_username|
|Signal Name|Suspicious Writes To Windows Recycle Bin|
|Summary Expression|Write to Recycle Bin by non-explorer process on host: {{device_hostname}}|
|Score/Severity|Static: 1|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0002, _mitreAttackTactic:TA0009, _mitreAttackTechnique:T1059, _mitreAttackTechnique:T1059.003, _mitreAttackTechnique:T1074, _mitreAttackTechnique:T1074.001|
## Vendors and Products
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|baseImage|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|file_path|
|Normalized Schema|lower|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|user_username|


