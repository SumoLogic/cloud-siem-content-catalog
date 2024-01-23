# [Rules](README.md): Microsoft Office Add-In Persistence

## Description
Detects additions to Microsoft Office add-ins on a host. Add-ins can be used by an adversary to gain poersistence as they are executed on Office applications being launched.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Persistence|
|Apply Risk to Entities|device_hostname|
|Signal Name|Microsoft Office Add-In Persistence|
|Summary Expression|Detected Office Add-In Addition activity on host: {{device_hostname}}|
|Score/Severity|Static: 2|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0003, _mitreAttackTechnique:T1137.006, _mitreAttackTechnique:T1137|
## Vendors and Products
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|changeTarget|
|Normalized Schema|device_hostname|


