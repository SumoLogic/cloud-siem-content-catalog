# [Rules](README.md): Windows - Powershell Scheduled Task Creation from PowerSploit or Empire

## Description
This rule detects the creation of a Windows scheduled task via PowerSploit or the default configuration of Empire.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Persistence|
|Apply Risk to Entities|device_hostname, device_ip, user_username|
|Signal Name|Windows - Powershell Scheduled Task Creation from PowerSploit or Empire|
|Summary Expression|Parent process: {{parentBaseImage}} spawned process: {{baseImage}} on host: {{device_hostname}}|
|Score/Severity|Static: 4|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0002, _mitreAttackTactic:TA0003, _mitreAttackTactic:TA0004, _mitreAttackTechnique:T1053, _mitreAttackTechnique:T1053.002, _mitreAttackTechnique:T1053.005|
## Vendors and Products
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|commandLine|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|parentBaseImage|
|Normalized Schema|user_username|


