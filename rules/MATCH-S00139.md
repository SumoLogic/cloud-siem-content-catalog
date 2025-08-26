# [Rules](README.md): Abnormal Parent-Child Process Combination

## Description
This alert detects a Windows process spawned by a parent process that does not normally spawn it.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Execution|
|Apply Risk to Entities|device_ip, user_username, device_hostname|
|Signal Name|Abnormal Parent-Child Process Combination|
|Summary Expression|Process: {{baseImage}} spawned by Parent Process: {{parentBaseImage}} on host: {{device_hostname}} by user: {{user_username}}|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0002, _mitreAttackTactic:TA0005, _mitreAttackTechnique:T1036, _mitreAttackTechnique:T1036.004, _mitreAttackTechnique:T1036.005|
## Vendors and Products
- [CrowdStrike - FDR](../products/569a3a44-c29f-492e-bcf4-5dc04e2ab0f3.md)
- [CrowdStrike - Filevantage](../products/a1f79987-b765-4f6f-bfe5-d657baa35144.md)
- [Microsoft - Azure](../products/a1225af5-e778-4068-a9a2-47da93d1ff24.md)
- [Microsoft - Office 365](../products/d3ed003d-5ddd-4c7a-bea5-63eae6311833.md)
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)
- [VMware - Carbon Black Cloud](../products/f9cea291-9030-4e41-9836-6dd9274d6df4.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|baseImage|
|Normalized Schema|commandLine|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|parentBaseImage|
|Normalized Schema|user_username|


