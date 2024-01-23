# [Rules](README.md): Azorult Malware Registry Key

## Description
Observes for a Windows registry key associated with Azorult malware on a system

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Unknown/Other|
|Apply Risk to Entities|device_hostname, user_username|
|Signal Name|Azorult Malware Registry Key|
|Summary Expression|A registry key associated with Azorult malware has been detected on {{device_hostname}}|
|Score/Severity|Static: 4|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0004, _mitreAttackTechnique:T1134, _mitreAttackTechnique:T1134.002|
## Vendors and Products
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|device_hostname|
|Normalized Schema|file_path|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|user_username|


