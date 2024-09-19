# [Rules](README.md): Loadable Kernel Module Dependency Install

## Description
Detects commands associated with the installation of loadable kernel modules. LKMs can be used on Linux systems to accomplish persistence by modifying the kernel to execute malicious programs at boot automatically.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Persistence|
|Apply Risk to Entities|device_hostname, device_ip, user_username|
|Signal Name|Loadable Kernel Module Dependency Install|
|Summary Expression|LKM dependency install detected on host: {{device_hostname}}|
|Score/Severity|Static: 2|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0003, _mitreAttackTechnique:T1547.006|
## Vendors and Products
- [Linux - Linux OS Syslog](../products/0e20c932-d992-4bd4-b276-c15119ca5c0b.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|commandLine|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|user_username|


