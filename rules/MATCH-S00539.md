# [Rules](README.md): Web Servers Executing Suspicious Processes

## Description
This rule looks for suspicious processes on all systems labeled as web servers. A list of web servers should be populated in order to enable the rule.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Defense Evasion|
|Apply Risk to Entities|device_hostname, device_ip, user_username|
|Signal Name|Web Servers Executing Suspicious Processes|
|Summary Expression|Suspicious process detected on host: {{device_hostname}} designated a web server|
|Score/Severity|Static: 4|
|Enabled by Default|False|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0003, _mitreAttackTechnique:T1505, _mitreAttackTechnique:T1505.003|
## Vendors and Products
- [Microsoft - Azure](../products/a1225af5-e778-4068-a9a2-47da93d1ff24.md)
- [Microsoft - Defender Advanced Hunting](../products/3382523e-2072-41bd-b50b-6b148957d0b0.md)
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|commandLine|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|listMatches|
|Normalized Schema|user_username|


