# [Rules](README.md): Potential Microsoft Office Template Abuse

## Description
Detects modifications to files and registry entries related to Microsoft Office Template Macros. These can be abused by an adversary to gain persistence.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Persistence|
|Apply Risk to Entities|device_hostname|
|Signal Name|Potential Microsoft Office Template Abuse|
|Summary Expression|Potential Office Template Abuse detected on host: {{device_hostname}}|
|Score/Severity|Static: 4|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0003, _mitreAttackTechnique:T1137, _mitreAttackTechnique:T1137.001|
## Vendors and Products
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|changeTarget|
|Normalized Schema|device_hostname|


