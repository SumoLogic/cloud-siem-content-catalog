# [Rules](README.md): Impacket Lateralization Detection

## Description
Detects wmiexec/dcomexec/atexec/smbexec from Impacket framework

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Lateral Movement|
|Apply Risk to Entities|device_hostname, device_ip, user_username|
|Signal Name|Impacket Lateralization Detection|
|Summary Expression|Impacket lateralization detected on command line from user: {{user_username}} on host: {{device_hostname}}|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0002, _mitreAttackTactic:TA0008, _mitreAttackTechnique:T1021, _mitreAttackTechnique:T1021.002, _mitreAttackTechnique:T1021.003, _mitreAttackTechnique:T1021.006, _mitreAttackTechnique:T1047, _mitreAttackTechnique:T1559, _mitreAttackTechnique:T1559.001|
## Vendors and Products
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|baseImage|
|Normalized Schema|commandLine|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|user_username|


