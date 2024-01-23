# [Rules](README.md): PXELoot Utility

## Description
From FireEye Red Team Tool Countermeasures:
PXELoot (PAL) is a C# tool designed to aid in the discovery and exploitation of misconfigurations in Windows Deployment Services (WDS).

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Discovery|
|Apply Risk to Entities|device_hostname, user_username|
|Signal Name|PXELoot Utility|
|Summary Expression|PXELoot indicators detected on host: {{device_hostname}}|
|Score/Severity|Static: 5|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0007, _mitreAttackTechnique:T1018|
## Vendors and Products
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|baseImage|
|Normalized Schema|commandLine|
|Normalized Schema|device_hostname|
|Normalized Schema|file_path|
|Normalized Schema|user_username|


