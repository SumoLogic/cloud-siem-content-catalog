# [Rules](README.md): Excessive Use of Escape Characters in Command Line

## Description
Fluffing a malicious command line input with escape characters is sometimes done in an attempt to avoid endpoint monitoring techniques that rely on exact string or regex matches.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Defense Evasion|
|Apply Risk to Entities|user_username, device_hostname, device_ip|
|Signal Name|Excessive Use of Escape Characters in Command Line|
|Summary Expression|A command with an excessive number of escape characters was executed on host {{device_hostname}} by user {{user_username}}|
|Score/Severity|Static: 5|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0005, _mitreAttackTechnique:T1027, _mitreAttackTechnique:T1027.002, _mitreAttackTechnique:T1027.004|
## Vendors and Products
- [Linux - Linux OS Syslog](../products/0e20c932-d992-4bd4-b276-c15119ca5c0b.md)
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|commandLine|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|user_username|


