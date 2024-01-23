# [Rules](README.md): Azure - Virtual Machine Stopped

## Description
Detects a virtual machine starting in Azure. This is most likely routine activity, however virtual machines may also be used for malicious activity.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Impact|
|Apply Risk to Entities|device_ip, user_username|
|Signal Name|Azure - Virtual Machine Stopped|
|Summary Expression|Azure Virtual Machine stopped by user: {{user_username}} resource: {{resource}}|
|Score/Severity|Static: 2|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTechnique:T1578, _mitreAttackTechnique:T1578.004, _mitreAttackTactic:TA0040|
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


