# [Rules](README.md): New or Renamed Windows User Account Mimicking a Machine Account

## Description
A new or renamed user account which starts with a $ following machine account naming conventions.  Attackers could use this to bypass detection logic where machine names are filtered from rules.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Persistence|
|Apply Risk to Entities|device_ip, user_username, device_hostname|
|Signal Name|New or Renamed Windows User Account Mimicking a Machine Account|
|Summary Expression|User: {{user_username}} may be masquerading as a machine account|
|Score/Severity|Static: 1|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0003, _mitreAttackTactic:TA0005, _mitreAttackTechnique:T1036, _mitreAttackTechnique:T1036.003, _mitreAttackTechnique:T1036.004, _mitreAttackTechnique:T1036.005|
## Vendors and Products
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|changeTarget|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Direct from Record|fields['EventData.NewTargetUserName']|
|Direct from Record|fields['EventData.OldTargetUserName']|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|user_username|


