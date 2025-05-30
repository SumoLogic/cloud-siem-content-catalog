# [Rules](README.md): Meterpreter or Cobalt Strike Getsystem Service Start

## Description
Detects the use of getsystem Meterpreter/Cobalt Strike command by detecting a specific service starting.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Privilege Escalation|
|Apply Risk to Entities|device_hostname, device_ip, user_username|
|Signal Name|Meterpreter or Cobalt Strike Getsystem Service Start|
|Summary Expression|Meterpreter/Cobalt Strike command detected on host: {{device_hostname}}|
|Score/Severity|Static: 4|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0003, _mitreAttackTactic:TA0004, _mitreAttackTechnique:T1543, _mitreAttackTechnique:T1569, _mitreAttackTechnique:T1543.003, _mitreAttackTechnique:T1569.002|
## Vendors and Products
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|commandLine|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|lower|
|Normalized Schema|parentBaseImage|
|Normalized Schema|user_username|


