# [Rules](README.md): Zoom Child Process

## Description
Observes for Zoom creating child processes

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Execution|
|Apply Risk to Entities|device_hostname, user_username|
|Signal Name|Zoom Child Process|
|Summary Expression|Detected Zoom spawning child process: {{baseImage}} on host: {{device_hostname}}|
|Score/Severity|Static: 1|
|Enabled by Default|True|
|Prototype|True|
|Tags|_mitreAttackTactic:TA0002|
## Vendors and Products
- [CrowdStrike - FDR](../products/569a3a44-c29f-492e-bcf4-5dc04e2ab0f3.md)
- [Digital Guardian - ARC](../products/975d678e-eb46-4155-9427-0fa307971fcd.md)
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


