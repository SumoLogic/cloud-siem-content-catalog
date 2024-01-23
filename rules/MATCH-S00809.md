# [Rules](README.md): Azure - Container Start

## Description
Detects Azure container starts. An adversary may use containers for malicious activity or to evade detection.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Execution|
|Apply Risk to Entities|device_ip, user_username|
|Signal Name|Azure - Container Start|
|Summary Expression|An Azure Container was started by user: {{user_username}} resource: {{resource}}|
|Score/Severity|Static: 1|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0002, _mitreAttackTactic:TA0005, _mitreAttackTechnique:T1610, _mitreAttackTechnique:T1204, _mitreAttackTechnique:T1204.003|
## Vendors and Products
- [Microsoft - Azure](../products/a1225af5-e778-4068-a9a2-47da93d1ff24.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|description|
|Normalized Schema|device_ip|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|success|
|Normalized Schema|user_username|


