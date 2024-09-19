# [Rules](README.md): Suspicious Non-Standard InstallUtil Execution

## Description
From FireEye Red Team Tool Countermeasures:
This alert looks for evidence of the native signed Windows binary InstallUtil.exe being used to load PE files. This technique can be used to bypass application whitelisting and has been observed used in the wild.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Defense Evasion|
|Apply Risk to Entities|device_hostname, user_username|
|Signal Name|Suspicious Non-Standard InstallUtil Execution|
|Summary Expression|Suspicious InstallUtil Execution - Parent process: {{parentBaseImage}} spawned process: {{baseImage}} on host: {{device_hostname}}|
|Score/Severity|Static: 5|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0005, _mitreAttackTechnique:T1218, _mitreAttackTechnique:T1218.007|
## Vendors and Products
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|baseImage|
|Normalized Schema|commandLine|
|Normalized Schema|device_hostname|
|Normalized Schema|parentBaseImage|
|Normalized Schema|user_username|


