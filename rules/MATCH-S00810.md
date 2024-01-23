# [Rules](README.md): Azure - Image Deleted

## Description
Detects deletions of Azure images. An adversary may try to destroy data or compromise backups by deleting an image.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Impact|
|Apply Risk to Entities|device_ip, user_username|
|Signal Name|Azure - Image Deleted|
|Summary Expression|An Azure Image was deleted by user: {{user_username}} resource: {{resource}}|
|Score/Severity|Static: 2|
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
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|success|
|Normalized Schema|user_username|


