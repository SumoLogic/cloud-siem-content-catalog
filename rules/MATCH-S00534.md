# [Rules](README.md): MacOS - Re-Opened Applications

## Description
This rule looks for processes referencing the plist files that determine which applications are re-opened when a user reboots their machine. This may also detect commands associated with login hooks being executed.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Persistence|
|Apply Risk to Entities|device_hostname, device_ip, user_username|
|Signal Name|MacOS - Re-Opened Applications|
|Summary Expression|Startup file referenced on host: {{device_hostname}}|
|Score/Severity|Static: 1|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0003, _mitreAttackTactic:TA0004, _mitreAttackTechnique:T1547, _mitreAttackTechnique:T1647, _mitreAttackTechnique:T1547.007, _mitreAttackTechnique:T1543.004, _mitreAttackTechnique:T1543.001, _mitreAttackTechnique:T1543, _mitreAttackTechnique:T1037.002, _mitreAttackTechnique:T1037|
## Vendors and Products
- [Carbon Black - Defense](../products/4448ca62-bb4f-4859-a6a2-d9262f9e48f0.md)
- [CrowdStrike - FDR](../products/569a3a44-c29f-492e-bcf4-5dc04e2ab0f3.md)
- [Microsoft - Azure](../products/a1225af5-e778-4068-a9a2-47da93d1ff24.md)
- [Microsoft - Defender Advanced Hunting](../products/3382523e-2072-41bd-b50b-6b148957d0b0.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|commandLine|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|user_username|


