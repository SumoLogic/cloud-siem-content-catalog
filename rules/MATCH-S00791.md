# [Rules](README.md): Azure - Secret Deleted

## Description
Detects deletions of Azure Key Vault Secrets. If a secret is not backed up or otherwise recoverable (see soft delete) it may render content indecipherable, leading to data loss.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Credential Access|
|Apply Risk to Entities|device_ip, user_username|
|Signal Name|Azure - Secret Deleted|
|Summary Expression|An Azure Key Vault Secret was deleted by user: {{user_username}} resource: {{resource}}|
|Score/Severity|Static: 5|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0006, _mitreAttackTactic:TA0040, _mitreAttackTechnique:T1485, _mitreAttackTechnique:T1552.005, _mitreAttackTechnique:T1552.004, _mitreAttackTechnique:T1552|
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


