# [Rules](README.md): Sunburst Suspicious File Writes

## Description
From FireEye Sunburst Countermeasures:
This rule identifies writes of specific file types associated with activity related to the SUNBURST backdoored version of the SolarWinds.Orion.Core.BusinessLayer.dll process. This rule may generate false positives depending on the configuration of SolarWinds in a given environment, and may require tuning to exclude legitimate activity. SUNBURST is a backdoor that has the ability to spawn and kill processes, write and delete files, set and create registry keys, gather system information, and disable a set of forensic analysis tools and services.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Initial Access|
|Apply Risk to Entities|device_hostname, user_username|
|Signal Name|Sunburst Suspicious File Writes|
|Summary Expression|Suspicious file written: {{file_path}}|
|Score/Severity|Static: 5|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0001, _mitreAttackTechnique:T1195, _mitreAttackTechnique:T1195.001, _mitreAttackTechnique:T1195.002|
## Vendors and Products
- [Microsoft - Azure](../products/a1225af5-e778-4068-a9a2-47da93d1ff24.md)
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|baseImage|
|Normalized Schema|device_hostname|
|Normalized Schema|file_path|
|Normalized Schema|user_username|


