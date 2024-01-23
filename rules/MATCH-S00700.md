# [Rules](README.md): KeePass Brute Force Tool Detection

## Description
Detects the use of a PowerShell KeePass brute force tool used in a dictionary attack to find and dump the passwords of a KeePass kdbx file.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Credential Access|
|Apply Risk to Entities|device_hostname, device_ip, user_username|
|Signal Name|KeePass Brute Force Tool Detection|
|Summary Expression|KeePass Brute Force Tool Detected on host: {{device_hostname}} IP: {{device_ip}} with user: {{user_username}}|
|Score/Severity|Static: 4|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0006, _mitreAttackTechnique:T1555, _mitreAttackTechnique:T1555.005|
## Vendors and Products
- [Linux - Linux OS Syslog](../products/0e20c932-d992-4bd4-b276-c15119ca5c0b.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|commandLine|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|user_username|


