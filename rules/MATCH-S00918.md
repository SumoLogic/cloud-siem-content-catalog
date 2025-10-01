# [Rules](README.md): Suspicious cat of PAM common-password policy

## Description
The Pluggable Authentication Module (PAM) in Linux allows system administrators to choose how applications authenticate users. The common-password file defines behavior of password use in Linux subsystems. This detection looks for use of cat to display the contents of the common-password file, which should not be a common occurrence on systems. It is recommended to investigate the host upon which this detection occurs to understand the exposure of the password policies for the system.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Discovery|
|Apply Risk to Entities|device_hostname, device_ip, user_username|
|Signal Name|Suspicious cat of PAM common-password policy on {{device_hostname}}|
|Summary Expression|User: {{user_username}} ran cat on pam.d common-password on {{device_hostname}}|
|Score/Severity|Static: 2|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0007, _mitreAttackTechnique:T1201|
## Vendors and Products
- [CrowdStrike - FDR](../products/569a3a44-c29f-492e-bcf4-5dc04e2ab0f3.md)
- [Linux - Linux OS Syslog](../products/0e20c932-d992-4bd4-b276-c15119ca5c0b.md)
- [Linux - Sysmon for Linux](../products/b238758d-ade8-41d2-b32d-c99159e9fd74.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|commandLine|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|user_username|


