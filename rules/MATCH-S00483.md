# [Rules](README.md): Impacket-Obfuscation WMIEXEC Utility

## Description
From FireEye Red Team Tool Countermeasures: Impacket-Obfuscation is a slightly obfuscated version of the open source Impacket framework. This IOC looks for artifacts from the execution of WMIEXEC python script which is part of Impacket-Obfuscation framework.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Execution|
|Apply Risk to Entities|device_hostname, device_ip, user_username|
|Signal Name|Impacket-Obfuscation WMIEXEC Utility|
|Summary Expression|Impacket obfuscation detected from user: {{user_username}} on host: {{device_hostname}}|
|Score/Severity|Static: 5|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0002, _mitreAttackTechnique:T1047|
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
|Normalized Schema|parentBaseImage|
|Normalized Schema|user_username|


