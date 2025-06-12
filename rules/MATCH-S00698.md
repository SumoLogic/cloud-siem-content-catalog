# [Rules](README.md): PATH Set to Current Directory

## Description
The PATH environment variable should always be set to an absolute directory pathing. Referencing the current directory is considered bad practice as it can lead to unintentional file execution or malicious abuse, as with CVE-2021-4034 (pkexec privilege escalation).

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Privilege Escalation|
|Apply Risk to Entities|device_hostname, user_username|
|Signal Name|PATH Variable Set to Current Directory|
|Summary Expression|User: {{user_username}} executed a command on host {{device_hostname}} to set the PATH variable|
|Score/Severity|Static: 4|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0004, _mitreAttackTechnique:T1574, _mitreAttackTechnique:T1574.007|
## Vendors and Products
- [CrowdStrike - FDR](../products/569a3a44-c29f-492e-bcf4-5dc04e2ab0f3.md)
- [CrowdStrike - Falcon](../products/840c72e0-4e47-41e7-9b93-31f55d12f07d.md)
- [Linux - Linux OS Syslog](../products/0e20c932-d992-4bd4-b276-c15119ca5c0b.md)
- [Microsoft - Azure](../products/a1225af5-e778-4068-a9a2-47da93d1ff24.md)
- [Microsoft - Defender Advanced Hunting](../products/3382523e-2072-41bd-b50b-6b148957d0b0.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|commandLine|
|Normalized Schema|device_hostname|
|Normalized Schema|user_username|


