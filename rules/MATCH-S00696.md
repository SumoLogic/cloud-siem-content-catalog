# [Rules](README.md): DPAPI Key Manipulation - Extracting Backup Key

## Description
The DPAPI (Data Protection Application Programming Interface) Key is used to encrypt user details. Actors may attempt to attack the DPAPI on the Domain Controllers to gain further access.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Credential Access|
|Apply Risk to Entities|device_hostname, user_username|
|Signal Name|DPAPI Key Manipulation - Extracting Backup Key|
|Summary Expression|Attempt to extract backup key on host: {{device_hostname}} by user: {{user_username}}|
|Score/Severity|Static: 2|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0006, _mitreAttackTechnique:T1003, _mitreAttackTechnique:T1555, _mitreAttackTechnique:T1555.003|
## Vendors and Products
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|changeTarget|
|Normalized Schema|device_hostname|
|Direct from Record|fields['EventData.AccessMask']|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|resource|
|Normalized Schema|user_username|


