# [Rules](README.md): TAIDOOR RAT DLL Load

## Description
Looks for process creation with command line references that are consistent with the Chinese TAIDOOR remote access trojan (RAT)

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Command and Control|
|Apply Risk to Entities|device_hostname, device_ip, user_username|
|Signal Name|TAIDOOR RAT DLL Load|
|Summary Expression|RAT activity on host: {{device_hostname}}|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0004, _mitreAttackTactic:TA0005, _mitreAttackTactic:TA0011, _mitreAttackTechnique:T1055, _mitreAttackTechnique:T1055.001, _mitreAttackTechnique:T1129|
## Vendors and Products
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|commandLine|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|user_username|


