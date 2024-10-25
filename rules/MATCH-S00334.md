# [Rules](README.md): Judgement Panda Exfil Activity

## Description
Detects Judgement Panda activity as described in Global Threat Report 2019 by Crowdstrike

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Execution|
|Apply Risk to Entities|device_hostname, device_ip, user_username|
|Signal Name|Judgement Panda Exfil Activity|
|Summary Expression|Judgement Panda exfiltration activity detected from process: {{baseImage}} on host: {{device_hostname}}|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0002, _mitreAttackTactic:TA0006, _mitreAttackTactic:TA0009, _mitreAttackTechnique:T1003, _mitreAttackTechnique:T1003.002, _mitreAttackTechnique:T1560, _mitreAttackTechnique:T1560.001|
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


