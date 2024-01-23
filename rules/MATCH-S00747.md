# [Rules](README.md): Registry Modification - Active Setup

## Description
Detects modifications to the active setup registry key. Active setup can be used to execute programs at user login.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Persistence|
|Apply Risk to Entities|device_hostname|
|Signal Name|Registry Modification - Active Setup|
|Summary Expression|Windows Active Setup registry modified on host: {{device_hostname}}|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0003, _mitreAttackTechnique:T1547.014|
## Vendors and Products
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|changeTarget|
|Normalized Schema|device_hostname|


