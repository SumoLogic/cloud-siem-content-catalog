# [Rules](README.md): Azure - Storage Modification

## Description
Detects modifications within an Azure Storage Account. Write events encapsulate both creations and changes to existing objects. Creation or modifications of shares and public storage blobs may indicate exfiltration attempts.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Exfiltration|
|Apply Risk to Entities|device_ip, user_username|
|Signal Name|Azure - {{description}}|
|Summary Expression|An Azure Storage Account object was created or modified by user: {{user_username}}  resource: {{resource}}|
|Score/Severity|Static: 1|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0010, _mitreAttackTechnique:T1530|
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


