# [Rules](README.md): Windows - Network Connection from CMSTP

## Description
Detects potential CMSTP.exe abuse. Adversaries use CMSTP.exe to load and execute DLLs or COM scriptlets from remote servers to bypass application control defenses.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Defense Evasion|
|Apply Risk to Entities|device_hostname, device_ip, user_username|
|Signal Name|Windows - Network Connection from CMSTP|
|Summary Expression|Network connected from CMSTP on host: {{device_hostname}}|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0005, _mitreAttackTechnique:T1218, _mitreAttackTechnique:T1218.003|
## Vendors and Products
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|dstDevice_ip_isInternal|
|Normalized Schema|file_path|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|srcDevice_hostname|
|Normalized Schema|user_username|


