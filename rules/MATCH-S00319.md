# [Rules](README.md): Dridex Process Pattern

## Description
Detects typical Dridex process patterns

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Execution|
|Apply Risk to Entities|device_hostname, device_ip, user_username|
|Signal Name|Dridex Process Pattern|
|Summary Expression|A suspicious command execution was observed on host: {{device_hostname}}|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0002, _mitreAttackTactic:TA0005, _mitreAttackTactic:TA0007, _mitreAttackTactic:TA0040, _mitreAttackTechnique:T1083, _mitreAttackTechnique:T1222, _mitreAttackTechnique:T1222.001, _mitreAttackTechnique:T1486, _mitreAttackTechnique:T1490|
## Vendors and Products
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|baseImage|
|Normalized Schema|commandLine|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|user_username|


