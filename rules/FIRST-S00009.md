# [Rules](README.md): First Seen RDP Logon From User

## Description
Observes for a user performing a RDP logon for the first time.

## Additional Details
|Detail|Value|
|----|----|
|Type|First Seen|
|Category|Lateral Movement|
|Apply Risk to Entities|user_username|
|Signal Name|First Seen RDP Logon From User|
|Summary Expression|First Seen RDP logon by the user: {{user_username}}|
|Retention Window|7776000000|
|Baseline Window|1814400000|
|Baseline Type|GLOBAL|
|Score/Severity|Static: 2|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0008, _mitreAttackTechnique:T1021, _mitreAttackTechnique:T1021.001|
## Vendors and Products
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Direct from Record|fields["EventData.LogonType"]|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|user_username|


