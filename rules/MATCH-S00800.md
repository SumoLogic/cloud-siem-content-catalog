# [Rules](README.md): Azure - Storage Deletion

## Description
Detects deletions within an Azure Storage Account.  Deletions of shares and public storage blobs may indicate data destruction.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Impact|
|Apply Risk to Entities|device_ip, user_username|
|Signal Name|Azure - {{description}}|
|Summary Expression|An Azure Storage Account object was deleted by user: {{user_username}}  resource: {{resource}}|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTechnique:T1530, _mitreAttackTechnique:T1485, _mitreAttackTactic:TA0040|
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


