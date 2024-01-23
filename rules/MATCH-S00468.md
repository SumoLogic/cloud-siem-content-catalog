# [Rules](README.md): SafetyKatz Credential Stealer

## Description
From FireEye Red Team Tool Countermeasures:
SafetyKatz is a combination of slightly modified version of Mimikatz project and .NET PE Loader.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Credential Access|
|Apply Risk to Entities|device_hostname, user_username|
|Signal Name|SafetyKatz Credential Stealer|
|Summary Expression|SafetyKatz credential stealer indicator detected on host: {{device_hostname}}|
|Score/Severity|Static: 5|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0006, _mitreAttackTechnique:T1003, _mitreAttackTechnique:T1003.001|
## Vendors and Products
- [Microsoft - Office 365](../products/d3ed003d-5ddd-4c7a-bea5-63eae6311833.md)
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|device_hostname|
|Normalized Schema|file_hash_md5|
|Normalized Schema|file_path|
|Normalized Schema|user_username|


