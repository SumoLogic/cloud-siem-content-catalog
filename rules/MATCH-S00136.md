# [Rules](README.md): PowerShell Encoded Command

## Description
PowerShell can execute encoded Base64 strings with the Encoded Command cmdlet. Attackers will often use Base64 to obfuscate their payloads until they can decode and execute it with PowerShell.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Execution|
|Apply Risk to Entities|device_hostname, device_ip, user_username|
|Signal Name|PowerShell Encoded Command|
|Summary Expression|Encoded Powershell command executed on host: {{device_hostname}}|
|Score/Severity|Static: 2|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0002, _mitreAttackTactic:TA0005, _mitreAttackTactic:TA0011, _mitreAttackTechnique:T1059, _mitreAttackTechnique:T1059.001, _mitreAttackTechnique:T1059.003, _mitreAttackTechnique:T1132, _mitreAttackTechnique:T1132.001, _mitreAttackTechnique:T1132.002, _mitreAttackTechnique:T1140|
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
|Normalized Schema|listMatches|
|Normalized Schema|user_username|


