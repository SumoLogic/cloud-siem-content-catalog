# [Rules](README.md): LSASS Memory Dumping

## Description
Detect creation of dump files containing the memory space of lsass.exe, which contains sensitive credentials. Identifies usage of Sysinternals procdump.exe to export the memory space of lsass.exe which contains sensitive credentials.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Credential Access|
|Apply Risk to Entities|device_hostname, device_ip, user_username|
|Signal Name|LSASS Memory Dumping|
|Summary Expression|LSASS memory dump detected on host: {{device_hostname}} from user: {{user_username}}|
|Score/Severity|Static: 4|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0006, _mitreAttackTechnique:T1003, _mitreAttackTechnique:T1003.001, _mitreAttackTechnique:T1003.007|
## Vendors and Products
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)
- [Tanium - Tanium Core](../products/5b49e894-92e8-45ad-8575-fe78b4f2e31b.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|baseImage|
|Normalized Schema|commandLine|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|lower|
|Normalized Schema|user_username|


