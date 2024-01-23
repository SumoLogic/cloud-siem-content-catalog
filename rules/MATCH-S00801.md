# [Rules](README.md): Azure - Virtual Machine Started

## Description
Detects a virtual machine starting in Azure. This is most likely routine activity, however virtual machines may also be used for malicious activity.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Persistence|
|Apply Risk to Entities|device_ip, user_username|
|Signal Name|Azure - Virtual Machine Started|
|Summary Expression|Azure Virtual Machine started by user: {{user_username}} resource: {{resource}}|
|Score/Severity|Static: 1|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0003, _mitreAttackTechnique:T1578, _mitreAttackTechnique:T1204, _mitreAttackTechnique:T1204.003|
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


