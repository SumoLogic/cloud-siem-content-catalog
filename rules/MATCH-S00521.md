# [Rules](README.md): Windows - Critical Service Disabled via Command Line

## Description
Detects a critical Windows service, such as Microsoft Defender or Windows Firewall, being stopped via the command line utilities sc.exe or net.exe. This could indicate an attacker attempting to bypass defenses on the target system to conduct further post-exploitation activity.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Defense Evasion|
|Apply Risk to Entities|device_hostname, device_ip, user_username|
|Signal Name|Windows - Critical Service Disabled via Command Line|
|Summary Expression|Critical Windows service stopped on host: {{device_hostname}} via command: {{commandline}}|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0005, _mitreAttackTechnique:T1562, _mitreAttackTechnique:T1562.001, _mitreAttackTechnique:T1562.002, _mitreAttackTechnique:T1562.004, _mitreAttackTechnique:T1562.006|
## Vendors and Products
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|commandLine|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|user_username|


