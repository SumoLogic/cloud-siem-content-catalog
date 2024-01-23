# [Rules](README.md): Suspect Svchost Activity

## Description
It is extremely abnormal for svchost.exe to spawn without any CLI arguments and is normally observed when a malicious process spawns the process and injects code into the process memory space.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Execution|
|Apply Risk to Entities|device_hostname, device_ip, user_username|
|Signal Name|Suspect Svchost Activity|
|Summary Expression|svchost spawned without arguments on host: {{device_hostname}}|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0002, _mitreAttackTactic:TA0004, _mitreAttackTactic:TA0005, _mitreAttackTechnique:T1055, _mitreAttackTechnique:T1055.001, _mitreAttackTechnique:T1055.002, _mitreAttackTechnique:T1055.003, _mitreAttackTechnique:T1055.004, _mitreAttackTechnique:T1055.009, _mitreAttackTechnique:T1055.012, _mitreAttackTechnique:T1055.013, _mitreAttackTechnique:T1569.002, _mitreAttackTechnique:T1569|
## Vendors and Products
- [CrowdStrike - FDR](../products/569a3a44-c29f-492e-bcf4-5dc04e2ab0f3.md)
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|baseImage|
|Normalized Schema|commandLine|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|parentBaseImage|
|Normalized Schema|user_username|


