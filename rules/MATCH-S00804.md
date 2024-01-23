# [Rules](README.md): Azure - Virtual Machine Deleted

## Description
Detects deletions of Azure virtual machines. Virtual machines may be deleted by an adversary to cover their tracks. Additionally, virtual machines might be deleted purely to cause damage.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Defense Evasion|
|Apply Risk to Entities|device_ip, user_username|
|Signal Name|Azure - Virtual Machine Deleted|
|Summary Expression|Azure Virtual Machine deleted by user: {{user_username}}  resource: {{resource}}|
|Score/Severity|Static: 2|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0005, _mitreAttackTactic:TA0040, _mitreAttackTechnique:T1578, _mitreAttackTechnique:T1578.003, _mitreAttackTechnique:T1485|
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


