# [Rules](README.md): RDP Login from Localhost

## Description
RDP login with a localhost source address may indicate a tunneled login and an attacker attempting to move through the environment.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Lateral Movement|
|Apply Risk to Entities|device_hostname, user_username|
|Signal Name|RDP Login from Localhost|
|Summary Expression|RDP connection from localhost on host: {{device_hostname}}|
|Score/Severity|Static: 4|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0001, _mitreAttackTactic:TA0003, _mitreAttackTactic:TA0004, _mitreAttackTactic:TA0005, _mitreAttackTactic:TA0008, _mitreAttackTechnique:T1078, _mitreAttackTechnique:T1078.003, _mitreAttackTechnique:T1078.002, _mitreAttackTechnique:T1078.001, _mitreAttackTechnique:T1021.001, _mitreAttackTechnique:T1021|
## Vendors and Products
- [CrowdStrike - FDR](../products/569a3a44-c29f-492e-bcf4-5dc04e2ab0f3.md)
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|logonType|
|Normalized Schema|objectType|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|user_username|


