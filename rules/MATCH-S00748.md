# [Rules](README.md): macOS Login Items Modification

## Description
Detects modifications to macOS login items. Login items are applications, files, folders, or connections which are launched upon user logon.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Persistence|
|Apply Risk to Entities|device_hostname|
|Signal Name|macOS Login Items Modification|
|Summary Expression|Detected Login Items Modification on host: {{device_hostname}}|
|Score/Severity|Static: 2|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0003, _mitreAttackTechnique:T1547.015|
## Vendors and Products


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|changeTarget|
|Normalized Schema|device_hostname|


