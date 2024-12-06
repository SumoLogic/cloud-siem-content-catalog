# [Rules](README.md): Malicious PowerShell Keywords

## Description
This rule detects well known keywords from PowerShell exploitation frameworks.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Execution|
|Apply Risk to Entities|user_username, device_hostname, device_ip|
|Signal Name|Malicious PowerShell Keywords|
|Summary Expression|Powershell exploitation keywords observed on host: {{device_hostname}}|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0002, _mitreAttackTactic:TA0006, _mitreAttackTechnique:T1003, _mitreAttackTechnique:T1003.001, _mitreAttackTechnique:T1003.002, _mitreAttackTechnique:T1003.003, _mitreAttackTechnique:T1003.004, _mitreAttackTechnique:T1003.005, _mitreAttackTechnique:T1059, _mitreAttackTechnique:T1059.003, _mitreAttackTechnique:T1059.001, _mitreAttackTechnique:T1134, _mitreAttackTechnique:T1134.001, _mitreAttackTechnique:T1134.002, _mitreAttackTechnique:T1134.003|
## Vendors and Products
- [CrowdStrike - FDR](../products/569a3a44-c29f-492e-bcf4-5dc04e2ab0f3.md)
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)
- [VMware - Carbon Black Cloud](../products/f9cea291-9030-4e41-9836-6dd9274d6df4.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|baseImage|
|Normalized Schema|commandLine|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|user_username|


