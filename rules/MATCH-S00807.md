# [Rules](README.md): Azure - Image Created/Modified

## Description
Detects creations or modifications of Azure images (Azure logs creations or modifications as write operations). Adversaries may attempt to create malicious images directly on a cloud deployment to avoid detection and establish persistence.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Persistence|
|Apply Risk to Entities|device_ip, user_username|
|Signal Name|Azure - Image Created/Modified|
|Summary Expression|An Azure image was created or modified by user: {{user_username}} resource: {{resource}}|
|Score/Severity|Static: 2|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0003, _mitreAttackTactic:TA0005, _mitreAttackTechnique:T1612, _mitreAttackTechnique:T1525, _mitreAttackTechnique:T1204, _mitreAttackTechnique:T1204.003|
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


