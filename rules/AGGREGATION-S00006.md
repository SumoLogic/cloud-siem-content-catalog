# [Rules](README.md): Docker Enumeration Detected on Host

## Description
Threat actors will aim to enumerate various permissions and settings on hosts with Docker installed, this enumeration can potentially lead to explotiation avenues.

## Additional Details
|Detail|Value|
|----|----|
|Type|Aggregation|
|Category|Discovery|
|Apply Risk to Entities|device_hostname|
|Signal Name|Docker Enumeration Detected on Host|
|Summary Expression|A number of Docker enumeration commands were issued on {{device_hostname}}|
|Aggregation Window|CUSTOM|
|Score/Severity|Static: 4|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0007, _mitreAttackTechnique:T1613|
## Vendors and Products
- [CrowdStrike - FDR](../products/569a3a44-c29f-492e-bcf4-5dc04e2ab0f3.md)
- [Linux - Linux OS Syslog](../products/0e20c932-d992-4bd4-b276-c15119ca5c0b.md)
- [Linux - Sysmon for Linux](../products/b238758d-ade8-41d2-b32d-c99159e9fd74.md)
- [Microsoft - Azure](../products/a1225af5-e778-4068-a9a2-47da93d1ff24.md)
- [Microsoft - Defender Advanced Hunting](../products/3382523e-2072-41bd-b50b-6b148957d0b0.md)
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|cmd_count|
|Normalized Schema|device_hostname|
|Normalized Schema|matches|
|Normalized Schema|metadata_deviceEventId|


