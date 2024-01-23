# [Rules](README.md): Ryuk Ransomware Endpoint Indicator

## Description
Indicates a process has started with charachteristics that are highly similar to the Ryuk ransomware's execution behavior.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Execution|
|Apply Risk to Entities|device_hostname, device_ip, user_username|
|Signal Name|Ryuk Ransomware Endpoint Indicator|
|Summary Expression|Ryuk ransomeware execution behavior detected on host: {{device_hostname}} in command: {{commandLine}}|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0002, _mitreAttackTactic:TA0003, _mitreAttackTactic:TA0004, _mitreAttackTechnique:T1547, _mitreAttackTechnique:T1547.001, _mitreAttackTechnique:T1059, _mitreAttackTechnique:T1486, _mitreAttackTechnique:T1059.003|
## Vendors and Products
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)
- [Tanium - Tanium Core](../products/5b49e894-92e8-45ad-8575-fe78b4f2e31b.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|commandLine|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|user_username|


