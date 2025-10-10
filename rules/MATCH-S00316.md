# [Rules](README.md): WannaCry Ransomware

## Description
Uses data from process creation events to detect indicators of the WannaCry Ransomware.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Execution|
|Apply Risk to Entities|device_hostname, device_ip, user_username|
|Signal Name|WannaCry Ransomware|
|Summary Expression|WannaCry ransomware indicator detected on host: {{device_hostname}}|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0002, _mitreAttackTactic:TA0005, _mitreAttackTactic:TA0007, _mitreAttackTactic:TA0008, _mitreAttackTactic:TA0040, _mitreAttackTechnique:T1083, _mitreAttackTechnique:T1210, _mitreAttackTechnique:T1222, _mitreAttackTechnique:T1222.001, _mitreAttackTechnique:T1486, _mitreAttackTechnique:T1490|
## Vendors and Products
- [CrowdStrike - FDR](../products/569a3a44-c29f-492e-bcf4-5dc04e2ab0f3.md)
- [CrowdStrike - Falcon](../products/840c72e0-4e47-41e7-9b93-31f55d12f07d.md)
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|baseImage|
|Normalized Schema|commandLine|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|user_username|


