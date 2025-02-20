# [Rules](README.md): First Seen Group Policy Discovery Operation

## Description
`This detection is a first observed execution of Windows process or PowerShell commands that can be run by users or administrators in order to gather password policy and other types of system information in an enterprise environment. The detections in this signal are based off variations found in Atomic Red Team test cases. Reference:  https://github.com/redcanaryco/atomic-red-team/blob/master/atomics/T1615/T1615.md. Look at the command line and parent process details of the signal in order to determine if this execution is legitimate or part of system provisioning or systems administration operations.

## Additional Details
|Detail|Value|
|----|----|
|Type|First Seen|
|Category|Discovery|
|Apply Risk to Entities|device_hostname, device_ip, user_username|
|Signal Name|First Seen Group Policy Discovery by {{user_username}}|
|Summary Expression|First Seen Group Policy Discovery on host: {{device_hostname}} by User: {{user_username}}|
|Retention Window|7776000000|
|Baseline Window|2592000000|
|Baseline Type|GLOBAL|
|Score/Severity|Static: 1|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0007, _mitreAttackTechnique:T1201|
## Vendors and Products
- [CrowdStrike - FDR](../products/569a3a44-c29f-492e-bcf4-5dc04e2ab0f3.md)
- [CrowdStrike - Falcon](../products/840c72e0-4e47-41e7-9b93-31f55d12f07d.md)
- [Microsoft - Azure](../products/a1225af5-e778-4068-a9a2-47da93d1ff24.md)
- [Microsoft - Defender Advanced Hunting](../products/3382523e-2072-41bd-b50b-6b148957d0b0.md)
- [Microsoft - Office 365](../products/d3ed003d-5ddd-4c7a-bea5-63eae6311833.md)
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|commandLine|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|user_username|


