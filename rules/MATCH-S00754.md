# [Rules](README.md): Registry Modification - Microsoft Office Test Function Registry Entry

## Description
Observes for modifications to the Microsoft Office Test registry key. This key allows for an arbitrary DLL to be executed on Office launch. This can be used by an adversary to establish persistence.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Persistence|
|Apply Risk to Entities|device_hostname|
|Signal Name|Registry Modification - Microsoft Office Test Function Registry Entry|
|Summary Expression|Observed Office Test Registry Modification on Host: {{device_hostname}}|
|Score/Severity|Static: 5|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0003, _mitreAttackTechnique:T1137, _mitreAttackTechnique:T1137.002|
## Vendors and Products
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|changeTarget|
|Normalized Schema|device_hostname|


