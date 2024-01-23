# [Rules](README.md): macOS - System Preference Enumeration via Security Binary

## Description
The security macOS binary was used to enumerate system settings, ensure that this activity is expected and authorized as system enumeration is performed by threat actors in order to discover misconfigurations or exploitation opportunities.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Discovery|
|Apply Risk to Entities|device_hostname|
|Signal Name|macOS - System Preference Enumeration via Security Binary|
|Summary Expression|macOS - System Preference Enumeration via Security Binary on {{device_hostname}}|
|Score/Severity|Static: 2|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0007, _mitreAttackTechnique:T1082|
## Vendors and Products


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|baseImage|
|Normalized Schema|device_hostname|


