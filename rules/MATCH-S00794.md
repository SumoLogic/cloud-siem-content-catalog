# [Rules](README.md): Azure - Secret Backup

## Description
Detects Secret backups within the Azure Key Vault. This may be an indication of data exfiltration and credential compromise.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Credential Access|
|Apply Risk to Entities|device_ip, user_username|
|Signal Name|Azure - Secret Backup|
|Summary Expression|Azure Key Vault Secret was backed up by user: {{user_username}} resource: {{resource}}|
|Score/Severity|Static: 2|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0006, _mitreAttackTactic:TA0010, _mitreAttackTechnique:T1555|
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


