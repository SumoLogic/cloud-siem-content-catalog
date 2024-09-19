# [Rules](README.md): First Seen vssadmin command From User

## Description
Threat actors may use the vssadmin utility to create volume shadow copies on a Windows operating system and retrieve the Active Directory database (NTDS.dit) file in order to extract credential material. This activity should be treated as high priority if not performed by an authorized systems administrator as part of normal and planned systems maintenance. If this activity is performed as part of normal system maintenance, the rule can be tuned to exclude these groups of users.

## Additional Details
|Detail|Value|
|----|----|
|Type|First Seen|
|Category|Defense Evasion|
|Apply Risk to Entities|user_username, device_hostname|
|Signal Name|First Seen vssadmin command  by {{user_username}}|
|Summary Expression|First Seen vssadmin command by User: {{user_username}} on the Host: {{device_hostname}}|
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


