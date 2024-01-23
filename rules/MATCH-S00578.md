# [Rules](README.md): Lsass Registry Key Modified

## Description
This rule monitors for changes to lsass.exe-related registry keys that are often edited to enable or obfuscate activity related to dumping the process.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Unknown/Other|
|Apply Risk to Entities|device_hostname, user_username|
|Signal Name|Lsass Registry Key Modified|
|Summary Expression|User {{user_username}} changed the registry key {{file_path}} on host {{device_hostname}}|
|Score/Severity|Static: 7|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0006, _mitreAttackTactic:TA0005, _mitreAttackTechnique:T1003, _mitreAttackTechnique:T1003.001, _mitreAttackTechnique:T1112|
## Vendors and Products
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|device_hostname|
|Normalized Schema|file_path|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|user_username|


