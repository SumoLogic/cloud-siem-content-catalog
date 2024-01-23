# [Rules](README.md): BlueMashroom DLL Load

## Description
Detects a suspicious DLL loading from AppData Local path as described in BlueMashroom report

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Execution|
|Apply Risk to Entities|device_hostname, device_ip, user_username|
|Signal Name|BlueMashroom DLL Load|
|Summary Expression|Suspicious DLL load detected on host: {{device_hostname}}|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0003, _mitreAttackTactic:TA0004, _mitreAttackTactic:TA0005, _mitreAttackTechnique:T1574, _mitreAttackTechnique:T1574.002, _mitreAttackTechnique:T1055, _mitreAttackTechnique:T1055.001, _mitreAttackTechnique:T1129|
## Vendors and Products
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|commandLine|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|lower|
|Normalized Schema|user_username|


