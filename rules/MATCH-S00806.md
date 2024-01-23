# [Rules](README.md): Azure - Bastion Host Deleted

## Description
Detects Azure bastion host deletions. An adversary might delete a bastion host to deny access to Azure resources.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Defense Evasion|
|Apply Risk to Entities|device_ip, user_username|
|Signal Name|Azure - Bastion Host Deleted|
|Summary Expression|An Azure Bastion Host was deleted by user {{user_username}} resource: {{resource}}|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0005, _mitreAttackTechnique:T1578, _mitreAttackTechnique:T1578.003, _mitreAttackTechnique:T1485|
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


