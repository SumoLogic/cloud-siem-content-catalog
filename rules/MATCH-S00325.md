# [Rules](README.md): Greenbug Campaign Indicators

## Description
Detects tools and process executions as observed in a Greenbug campaign in May 2020

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Execution|
|Apply Risk to Entities|device_hostname, device_ip, user_username|
|Signal Name|Greenbug Campaign Indicators|
|Summary Expression|Observed suspicious command execution on host: {{device_hostname}}|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0002, _mitreAttackTactic:TA0005, _mitreAttackTactic:TA0011, _mitreAttackTechnique:T1036, _mitreAttackTechnique:T1036.005, _mitreAttackTechnique:T1036.004, _mitreAttackTechnique:T1036.003, _mitreAttackTechnique:T1059, _mitreAttackTechnique:T1059.003, _mitreAttackTechnique:T1105|
## Vendors and Products
- [CrowdStrike - FDR](../products/569a3a44-c29f-492e-bcf4-5dc04e2ab0f3.md)
- [Microsoft - Defender Advanced Hunting](../products/3382523e-2072-41bd-b50b-6b148957d0b0.md)
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|baseImage|
|Normalized Schema|commandLine|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|user_username|


