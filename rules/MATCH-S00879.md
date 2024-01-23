# [Rules](README.md): macOS - Suspicious Osascript Execution

## Description
This alert looks for osascript execution with a suspicious parent process indicating execution from a shell or terminal

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Execution|
|Apply Risk to Entities|device_hostname|
|Signal Name|macOS - Suspicious Osascript Execution|
|Summary Expression|macOS - Suspicious Osascript Execution on {{device_hostname}}|
|Score/Severity|Static: 2|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0002, _mitreAttackTechnique:T1059.002|
## Vendors and Products


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|baseImage|
|Normalized Schema|device_hostname|


