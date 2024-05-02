# [Rules](README.md): Azure Authentication Policy Change

## Description
Various authentication related policy configurations exist within Azure - these are tenant-wide policy changes that affect aspects such as enabling of number matching, changing of which authentication methods users are allowed to use, or the exclusion of certain groups from various authentication methods.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Defense Evasion|
|Apply Risk to Entities|user_username|
|Signal Name|Azure Authentication Policy Modified|
|Summary Expression|{{user_username}} has changed an Azure Authentication Policy|
|Score/Severity|Static: 2|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0005, _mitreAttackTechnique:T1556|
## Vendors and Products
- [Microsoft - Azure](../products/a1225af5-e778-4068-a9a2-47da93d1ff24.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|action|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|user_username|


