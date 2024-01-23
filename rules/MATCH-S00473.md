# [Rules](README.md): SharpStomp Utility

## Description
From FireEye Red Team Tool Countermeasures:
SharpStomp is a C# utility that can be used to timestomp the specified file's creation, last access, and last write time.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Defense Evasion|
|Apply Risk to Entities|device_hostname, user_username|
|Signal Name|SharpStomp Utility|
|Summary Expression|SharpStomp Utility indicator detected on host: {{device_hostname}}|
|Score/Severity|Static: 5|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0005, _mitreAttackTechnique:T1070, _mitreAttackTechnique:T1070.006|
## Vendors and Products
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|baseImage|
|Normalized Schema|device_hostname|
|Normalized Schema|file_hash_md5|
|Normalized Schema|user_username|


