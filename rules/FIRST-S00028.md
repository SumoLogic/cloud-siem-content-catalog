# [Rules](README.md): First Seen Common Windows Recon Commands From User

## Description
Detects a set of commands often used in recon stages by different attack groups.

## Additional Details
|Detail|Value|
|----|----|
|Type|First Seen|
|Category|Discovery|
|Apply Risk to Entities|device_hostname, user_username|
|Signal Name|First Seen Common Windows Recon Commands From User|
|Summary Expression|Detected reconnaissance activity from user: {{user_username}} on host: {{device_hostname}}|
|Retention Window|7776000000|
|Baseline Window|1209600000|
|Baseline Type|GLOBAL|
|Score/Severity|Static: 2|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0007, _mitreAttackTechnique:T1018|
## Vendors and Products
- [Citrix - ADC](../products/d3606245-76d3-4173-a2fe-832c0e71b0f9.md)
- [CrowdStrike - FDR](../products/569a3a44-c29f-492e-bcf4-5dc04e2ab0f3.md)
- [CrowdStrike - Falcon](../products/840c72e0-4e47-41e7-9b93-31f55d12f07d.md)
- [Cylance - Protect](../products/60829f4a-7acb-47d1-ad23-8424fcf83dcb.md)
- [Linux - Linux OS Syslog](../products/0e20c932-d992-4bd4-b276-c15119ca5c0b.md)
- [Linux - Sysmon for Linux](../products/b238758d-ade8-41d2-b32d-c99159e9fd74.md)
- [Microsoft - Azure](../products/a1225af5-e778-4068-a9a2-47da93d1ff24.md)
- [Microsoft - Defender Advanced Hunting](../products/3382523e-2072-41bd-b50b-6b148957d0b0.md)
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|commandLine|
|Normalized Schema|device_hostname|
|Normalized Schema|listMatches|
|Normalized Schema|lower|
|Normalized Schema|parentBaseImage|
|Normalized Schema|user_username|


