# [Rules](README.md): Windows Disable Antispyware Registry

## Description
The rule looks for the Registry Key DisableAntiSpyware set to disable. This is consistent with Ryuk infections across a fleet of endpoints.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Defense Evasion|
|Apply Risk to Entities|device_hostname, device_ip, user_username|
|Signal Name|Windows Disable Antispyware Registry|
|Summary Expression|Ryuk ransomware indicator detected on host: {{device_hostname}}|
|Score/Severity|Static: 1|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0005, _mitreAttackTechnique:T1562, _mitreAttackTechnique:T1562.001, _mitreAttackTechnique:T1562.006|
## Vendors and Products
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Direct from Record|fields['EventData.Details']|
|Direct from Record|fields['EventData.NewValue']|
|Direct from Record|fields['EventData.NewValueType']|
|Direct from Record|fields['EventData.ObjectValueName']|
|Direct from Record|fields['insertionstrings_f08']|
|Normalized Schema|file_path|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|user_username|


