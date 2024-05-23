# [Rules](README.md): macOS - Keychain Enumeration

## Description
Threat actors may be able to list or acquire credentials from keychains, this alert looks for enumeration of available keychains on a given host.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Credential Access|
|Apply Risk to Entities|user_username|
|Signal Name|macOS - Keychain Enumeration on {{device_hostname}}|
|Summary Expression|macOS - Keychain Enumeration on {{device_hostname}} by {{user_username}}|
|Score/Severity|Static: 2|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0006, _mitreAttackTechnique:T1555.001|
## Vendors and Products


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|baseImage|
|Normalized Schema|device_hostname|
|Normalized Schema|matches|
|Normalized Schema|parentBaseImage|
|Normalized Schema|user_username|


