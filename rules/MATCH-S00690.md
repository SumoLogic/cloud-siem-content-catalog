# [Rules](README.md): Rundll32.exe Load from TEMP Directory with By Ordinal Load

## Description
Detects rundll32 loaded from a temp directory with a by ordinal load. This activity has been attributed to the Qbot and Bazar trojans.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Execution|
|Apply Risk to Entities|device_hostname, device_ip, user_username, srcDevice_hostname, srcDevice_ip|
|Signal Name|Rundll32.exe Load from TEMP Directory with By Ordinal Load|
|Summary Expression|Highly suspicious execution of rundll32.exe from TEMP detected on host: {{device_hostname}}|
|Score/Severity|Static: 10|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0002, _mitreAttackTechnique:T1059, _mitreAttackTechnique:T1059.003, _mitreAttackTactic:TA0005, _mitreAttackTechnique:T1218, _mitreAttackTechnique:T1218.011|
## Vendors and Products
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|baseImage|
|Normalized Schema|commandLine|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|srcDevice_hostname|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|user_username|


