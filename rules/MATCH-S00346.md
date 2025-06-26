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
|Summary Expression|Ryuk ransomeware execution behavior detected on host: {{device_hostname}}|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0002, _mitreAttackTactic:TA0003, _mitreAttackTactic:TA0004, _mitreAttackTechnique:T1547, _mitreAttackTechnique:T1547.001, _mitreAttackTechnique:T1059, _mitreAttackTechnique:T1486, _mitreAttackTechnique:T1059.003|
## Vendors and Products
- [CrowdStrike - Falcon](../products/840c72e0-4e47-41e7-9b93-31f55d12f07d.md)
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|commandLine|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|user_username|


