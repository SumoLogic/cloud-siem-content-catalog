# [Rules](README.md): macOS Startup Items Modifications

## Description
Detects modifications to startup items on a macOS system. Startup Items plist files can be used to establish persistence by an adversary.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Persistence|
|Apply Risk to Entities|device_hostname|
|Signal Name|macOS Startup Items Modifications|
|Summary Expression|Observed modifications to startup items on host: {{device_hostname}}|
|Score/Severity|Static: 4|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0003, _mitreAttackTechnique:T1037, _mitreAttackTechnique:T1037.005|
## Vendors and Products


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|changeTarget|
|Normalized Schema|device_hostname|


