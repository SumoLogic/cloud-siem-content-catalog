# [Rules](README.md): First Seen esentutl command From User

## Description
Threat actors may use the esentutl utility to create volume shadow copies and/or backups on a Windows operating system and retrieve the Active Directory database (NTDS.dit) file in order to extract credential material. Esentutl can also be utilized to download files from a remote share or URL. This activity should be treated as high priority if not performed by an authorized systems administrator as part of normal and planned systems maintenance.

## Additional Details
|Detail|Value|
|----|----|
|Type|First Seen|
|Category|Defense Evasion|
|Apply Risk to Entities|user_username, device_hostname|
|Signal Name|First Seen esentutl command  by {{user_username}}|
|Summary Expression|First Seen wbadmin command by User: {{user_username}} on Host: {{device_hostname}}|
|Retention Window|7776000000|
|Baseline Window|2592000000|
|Baseline Type|GLOBAL|
|Score/Severity|Static: 2|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0005, _mitreAttackTechnique:T1006|
## Vendors and Products
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|device_hostname|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|user_username|


