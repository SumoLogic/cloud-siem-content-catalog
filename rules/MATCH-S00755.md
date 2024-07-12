# [Rules](README.md): Outlook Form Creation

## Description
Detects Outlook Form creation.  Outlook forms can be used to execute code on a compromised machine and establish persistence.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Persistence|
|Apply Risk to Entities|device_hostname|
|Signal Name|Outlook Form Creation|
|Summary Expression|Observed Outlook Form creation on host: {{device_hostname}}|
|Score/Severity|Static: 1|
|Enabled by Default|True|
|Prototype|True|
|Tags|_mitreAttackTactic:TA0003, _mitreAttackTechnique:T1137, _mitreAttackTechnique:T1137.003|
## Vendors and Products
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|baseImage|
|Normalized Schema|changeTarget|
|Normalized Schema|device_hostname|


