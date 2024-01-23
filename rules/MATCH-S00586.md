# [Rules](README.md): Credential Dumping by LaZagne

## Description
Detects LSASS process access by LaZagne for credential dumping

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Unknown/Other|
|Apply Risk to Entities|device_hostname, user_username|
|Signal Name|Credential Dumping by LaZagne|
|Summary Expression|Observed LaZagne Credential Dumping behavior on. {{device_hostname}}|
|Score/Severity|Static: 5|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0006, _mitreAttackTechnique:T1003, _mitreAttackTechnique:T1003.001|
## Vendors and Products
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|device_hostname|
|Direct from Record|fields['EventData.CallTrace']|
|Direct from Record|fields['EventData.GrantedAccess']|
|Direct from Record|fields['EventData.TargetImage']|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|user_username|


