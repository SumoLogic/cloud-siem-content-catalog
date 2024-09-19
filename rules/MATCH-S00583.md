# [Rules](README.md): WCE wceaux.dll Access

## Description
Obvserves for access of wceaux.dll, which may be indicative of credential access.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Unknown/Other|
|Apply Risk to Entities|device_hostname, user_username|
|Signal Name|WCE wceaux.dll Access|
|Summary Expression|Access to wceaux.dll detected on {{device_hostname}}|
|Score/Severity|Static: 4|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0006, _mitreAttackTechnique:T1003, _mitreAttackTechnique:T1003.001, _mitreAttackTechnique:T1003.002, _mitreAttackTechnique:T1003.004, _mitreAttackTechnique:T1003.005, _mitreAttackTechnique:T1003.006|
## Vendors and Products
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|device_hostname|
|Direct from Record|fields['Eventdata.Objectname']|
|Normalized Schema|file_path|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|user_username|


