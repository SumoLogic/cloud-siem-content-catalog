# [Rules](README.md): Azure - Key Purged

## Description
Detects purges of Azure Key Vault Keys. If a key is not backed up it may render content indecipherable, leading to data loss. Key purges are performed on already deleted keys and must be explicitly allowed by the access policy as it redners them unrecoverable unless a backup was made.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Credential Access|
|Apply Risk to Entities|device_ip, user_username|
|Signal Name|Azure - Key Purged|
|Summary Expression|An Azure Key Vault Key was purged by user: {{user_username}} resource: {{resource}}|
|Score/Severity|Static: 7|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0006, _mitreAttackTactic:TA0040, _mitreAttackTechnique:T1485, _mitreAttackTechnique:T1552.004, _mitreAttackTechnique:T1552.005|
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


