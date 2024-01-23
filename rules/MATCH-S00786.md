# [Rules](README.md): Azure - SQL Database Export

## Description
A database export, especially to a public blob container, may indicate data exfiltration in progress.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Exfiltration|
|Apply Risk to Entities|device_ip, user_username|
|Signal Name|Azure - SQL Database Export|
|Summary Expression|Detected a database export by user: {{user_username}}  of resource: {{resource}}|
|Score/Severity|Static: 2|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0010, _mitreAttackTechnique:T1578.001, _mitreAttackTechnique:T1578|
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


