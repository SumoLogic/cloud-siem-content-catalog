# [Rules](README.md): Pkexec Privilege Escalation - CVE-2021-4034

## Description
Monitors for audit message and command line parameters that indicate attempted exploitation of pkexec vulnerability CVE-2021-4034.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Privilege Escalation|
|Apply Risk to Entities|device_hostname, user_username|
|Signal Name|Pkexec Privilege Escalation - CVE-2021-4034|
|Summary Expression|User: {{user_username}} executed a possible Pkexec command on host: {{device_hostname}}|
|Score/Severity|Static: 9|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0004, _mitreAttackTechnique:T1068|
## Vendors and Products
- [Linux - Linux OS Syslog](../products/0e20c932-d992-4bd4-b276-c15119ca5c0b.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|commandLine|
|Normalized Schema|description|
|Normalized Schema|device_hostname|
|Normalized Schema|user_username|


