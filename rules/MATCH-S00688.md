# [Rules](README.md): Bash History Tampering

## Description
This rule monitors for various methods of deleting or otherwise tampering with .bash_history files which store command history on Linux machines.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Defense Evasion|
|Apply Risk to Entities|device_hostname, device_ip, user_username|
|Signal Name|Bash History Tampering|
|Summary Expression|The command history on host {{device_hostname}} was manipulated by user {{user_username}}|
|Score/Severity|Static: 7|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0005, _mitreAttackTechnique:T1070, _mitreAttackTechnique:T1070.003|
## Vendors and Products
- [CrowdStrike - FDR](../products/569a3a44-c29f-492e-bcf4-5dc04e2ab0f3.md)
- [Linux - Linux OS Syslog](../products/0e20c932-d992-4bd4-b276-c15119ca5c0b.md)
- [Microsoft - Azure](../products/a1225af5-e778-4068-a9a2-47da93d1ff24.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|commandLine|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|user_username|


