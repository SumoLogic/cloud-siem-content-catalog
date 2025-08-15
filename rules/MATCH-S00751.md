# [Rules](README.md): Unix/Linux RC Script Modification

## Description
Detects modifications to RC Script files. These scripts are executed on system startup and may be used by an adversary to establish persistence.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Persistence|
|Apply Risk to Entities|device_hostname|
|Signal Name|Unix/Linux RC Script Modification|
|Summary Expression|RC Script modification detected on host: {{device_hostname}}|
|Score/Severity|Static: 4|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0003, _mitreAttackTechnique:T1037, _mitreAttackTechnique:T1037.004|
## Vendors and Products
- [Linux - Sysmon for Linux](../products/b238758d-ade8-41d2-b32d-c99159e9fd74.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|changeTarget|
|Normalized Schema|device_hostname|


