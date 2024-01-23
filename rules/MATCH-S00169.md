# [Rules](README.md): Windows - Microsoft Office Add-In File Created

## Description
This rule detects when a Microsoft Office Add-In is created by monitoring certain directories with specific file extensions. This rule requires the setup of file creation auditing.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Persistence|
|Apply Risk to Entities|device_hostname, device_ip, user_username|
|Signal Name|Windows - Microsoft Office Add-In File Created|
|Summary Expression|Microsoft Office add-in file created on host: {{device_hostname}}|
|Score/Severity|Static: 2|
|Enabled by Default|False|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0003, _mitreAttackTechnique:T1137, _mitreAttackTechnique:T1137.001, _mitreAttackTechnique:T1137.006|
## Vendors and Products
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|file_path|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|user_username|


