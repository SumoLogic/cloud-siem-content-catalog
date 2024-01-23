# [Rules](README.md): UserInit Process Launched by MSBuild.exe

## Description
From FireEye Red Team Tool Countermeasures:
MSBuild is the build system for Visual Studio. This IOC detects the suspicious execution of userinit process by MSBUILD.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Defense Evasion|
|Apply Risk to Entities|device_hostname, user_username|
|Signal Name|UserInit Process Launched by MSBuild.exe|
|Summary Expression|MSBuild launched userinit on host: {{device_hostname}}|
|Score/Severity|Static: 5|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0005, _mitreAttackTechnique:T1127, _mitreAttackTechnique:T1127.001|
## Vendors and Products
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|baseImage|
|Normalized Schema|device_hostname|
|Normalized Schema|parentBaseImage|
|Normalized Schema|user_username|


