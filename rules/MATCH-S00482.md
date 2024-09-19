# [Rules](README.md): Impacket-Obfuscation SMBEXEC Utility

## Description
From FireEye Red Team Tool Countermeasures: Impacket-Obfuscation is a slightly obfuscated version of the open source Impacket framework. This IOC looks for artifacts from the execution of SMBEXEC python script which is part of Impacket-Obfuscation framework.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Defense Evasion|
|Apply Risk to Entities|device_hostname, device_ip, user_username|
|Signal Name|Impacket-Obfuscation SMBEXEC Utility|
|Summary Expression|Impacket obfuscation detected from user: {{user_username}} on host: {{device_hostname}}|
|Score/Severity|Static: 5|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0003, _mitreAttackTactic:TA0004, _mitreAttackTactic:TA0005, _mitreAttackTactic:TA0008, _mitreAttackTechnique:T1021, _mitreAttackTechnique:T1021.002, _mitreAttackTechnique:T1021.006, _mitreAttackTechnique:T1036, _mitreAttackTechnique:T1036.004, _mitreAttackTechnique:T1036.005, _mitreAttackTechnique:T1543, _mitreAttackTechnique:T1543.003|
## Vendors and Products
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|baseImage|
|Normalized Schema|commandLine|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|file_path|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|parentBaseImage|
|Normalized Schema|user_username|


