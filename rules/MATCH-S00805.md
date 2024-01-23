# [Rules](README.md): Azure - Bastion Host Created/Modified

## Description
Detects Azure bastion host creations or modifications (Azure records a write operation for either). A new bastion host may be used by an adversary to gain persistence to Azure resources. Modifications of existing bastion hosts may indicate a compromise of these sensitive hosts.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Defense Evasion|
|Apply Risk to Entities|device_ip, user_username|
|Signal Name|Azure - Bastion Host Created/Modified|
|Summary Expression|An Azure Bastion Host was created or modified by user {{user_username}} resource: {{resource}}|
|Score/Severity|Static: 2|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0005, _mitreAttackTechnique:T1578, _mitreAttackTechnique:T1578.002|
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


