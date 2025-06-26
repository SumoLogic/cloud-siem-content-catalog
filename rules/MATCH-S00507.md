# [Rules](README.md): Spoolsv Child Process Created

## Description
Observes for Spoolsv launching unexpected child processes. This may be related to behavior in CVE-2018-8440

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Privilege Escalation|
|Apply Risk to Entities|device_hostname, user_username|
|Signal Name|Spoolsv Child Process Created|
|Summary Expression|Spoolsv.exe spawned child process: {{baseImage}}|
|Score/Severity|Static: 2|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0004, _mitreAttackTechnique:T1068|
## Vendors and Products
- [CrowdStrike - FDR](../products/569a3a44-c29f-492e-bcf4-5dc04e2ab0f3.md)
- [Microsoft - Azure](../products/a1225af5-e778-4068-a9a2-47da93d1ff24.md)
- [Microsoft - Defender Advanced Hunting](../products/3382523e-2072-41bd-b50b-6b148957d0b0.md)
- [Microsoft - Office 365](../products/d3ed003d-5ddd-4c7a-bea5-63eae6311833.md)
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)
- [VMware - Carbon Black Cloud](../products/f9cea291-9030-4e41-9836-6dd9274d6df4.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|baseImage|
|Normalized Schema|device_hostname|
|Normalized Schema|lower|
|Normalized Schema|parentBaseImage|
|Normalized Schema|user_username|


