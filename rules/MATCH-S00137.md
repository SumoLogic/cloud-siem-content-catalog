# [Rules](README.md): Office Application or Browser Launching Shell

## Description
This alert detects a shell launched by an office product or browser that should not be spawning shell processes. Attackers may inject code into Office documents or abuse Windows utilities to spawn shells that will execute malicious commands.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Execution|
|Apply Risk to Entities|device_ip, user_username, device_hostname|
|Signal Name|Office Application or Browser Launching Shell|
|Summary Expression|Office process: {{parentBaseImage}} spawned shell process: {{baseImage}}|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0001, _mitreAttackTactic:TA0002, _mitreAttackTactic:TA0043, _mitreAttackTechnique:T1204, _mitreAttackTechnique:T1204.001, _mitreAttackTechnique:T1204.002, _mitreAttackTechnique:T1204.003, _mitreAttackTechnique:T1566, _mitreAttackTechnique:T1566.001, _mitreAttackTechnique:T1566.002, _mitreAttackTechnique:T1566.003, _mitreAttackTechnique:T1598.001, _mitreAttackTechnique:T1598.002, _mitreAttackTechnique:T1598.003, _mitreAttackTechnique:T1598|
## Vendors and Products
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|baseImage|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|parentBaseImage|
|Normalized Schema|user_username|


