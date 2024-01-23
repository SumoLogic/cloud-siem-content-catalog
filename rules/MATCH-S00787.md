# [Rules](README.md): Azure - Protected Item Deletion Attempt

## Description
Detects the attempted deletion of protected items in Azure, such as backups. This may be an indicator of attempted data destruction.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Impact|
|Apply Risk to Entities|device_ip, user_username|
|Signal Name|Azure - Protected Item Deletion Attempt|
|Summary Expression|Attempted deletion of a protected item by user: {{user_username}}  of resource: {{resource}}|
|Score/Severity|Static: 1|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0040, _mitreAttackTechnique:T1485|
## Vendors and Products
- [Microsoft - Azure](../products/a1225af5-e778-4068-a9a2-47da93d1ff24.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|description|
|Normalized Schema|device_ip|
|Direct from Record|fields['resultType']|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|user_username|


