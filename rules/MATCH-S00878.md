# [Rules](README.md): macOS - Suspicious Osascript Parent Execution

## Description
This alert looks for osascript execution as the parent process indicating possible suspicious execution of a shell or terminal

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Execution|
|Apply Risk to Entities|user_username, device_hostname|
|Signal Name|macOS - Suspicious Osascript Parent Execution|
|Summary Expression|macOS - Suspicious Osascript Parent Execution on {{device_hostname}}|
|Score/Severity|Static: 1|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0002, _mitreAttackTechnique:T1059.002|
## Vendors and Products


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|device_hostname|
|Normalized Schema|lower|
|Normalized Schema|parentBaseImage|
|Normalized Schema|user_username|


