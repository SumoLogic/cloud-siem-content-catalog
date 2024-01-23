# [Rules](README.md): Windows Port Monitor Modification

## Description
Detects file creations or registry modifications to Windows port  monitors which can be used to gain persistence in a system process.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Persistence|
|Apply Risk to Entities|device_hostname|
|Signal Name|Windows Port Monitor Modification|
|Summary Expression|Port Monitor DLL detected on host: {{device_hostname}}|
|Score/Severity|Static: 5|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0003, _mitreAttackTechnique:T1547, _mitreAttackTechnique:T1547.010|
## Vendors and Products
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|baseImage|
|Normalized Schema|changeTarget|
|Normalized Schema|device_hostname|


