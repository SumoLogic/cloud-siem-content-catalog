# [Rules](README.md): Productivity App Spawning Rundll32 or Regsvr32

## Description
Detects productivity applications spawning regsvr32 or rundll32. This activity has been attributed to the Qbot and Bazar trojans.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Execution|
|Apply Risk to Entities|device_hostname, device_ip, user_username, srcDevice_hostname, srcDevice_ip|
|Signal Name|Productivity App Spawning Rundll32 or Regsvr32|
|Summary Expression|Productivity application process: {{parentBaseImage}} spawned child process: {{baseImage}}|
|Score/Severity|Static: 4|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0002, _mitreAttackTechnique:T1059, _mitreAttackTactic:TA0005, _mitreAttackTechnique:T1218, _mitreAttackTechnique:T1218.010, _mitreAttackTechnique:T1218.011, _mitreAttackTechnique:T1059.003|
## Vendors and Products
- [CrowdStrike - FDR](../products/569a3a44-c29f-492e-bcf4-5dc04e2ab0f3.md)
- [Microsoft - Azure](../products/a1225af5-e778-4068-a9a2-47da93d1ff24.md)
- [Microsoft - Defender Advanced Hunting](../products/3382523e-2072-41bd-b50b-6b148957d0b0.md)
- [Microsoft - Office 365](../products/d3ed003d-5ddd-4c7a-bea5-63eae6311833.md)
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|baseImage|
|Normalized Schema|commandLine|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|lower|
|Normalized Schema|parentBaseImage|
|Normalized Schema|srcDevice_hostname|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|user_username|


