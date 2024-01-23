# [Rules](README.md): Disabling Remote User Account Control

## Description
The rule looks for modifications to registry keys that control the enforcement of Windows User Account Control (UAC).

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Privilege Escalation|
|Apply Risk to Entities|device_hostname, device_ip, user_username|
|Signal Name|Disabling Remote User Account Control|
|Summary Expression|UAC registry modification on host: {{device_hostname}} by user: {{user_username}}|
|Score/Severity|Static: 1|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0004, _mitreAttackTactic:TA0005, _mitreAttackTechnique:T1548, _mitreAttackTechnique:T1548.002|
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


