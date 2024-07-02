# [Rules](README.md): Solarwinds Suspicious Child Processes

## Description
From FireEye Red Team Tool Countermeasures: This rule identifies suspicious child processes of SolarWinds.Orion.Core.BusinessLayer.dll that may be evidence of the SUNBURST backdoor. The behavior of SolarWinds.Orion.Core.BusinessLayer.dll is dependent on per-enterprise configuration, so additional tuning may be required to exclude legitimate activity in a given environment. SUNBURST is a backdoor that has the ability to spawn and kill processes, write and delete files, set and create registry keys, gather system information, and disable a set of forensic analysis tools and services.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Initial Access|
|Apply Risk to Entities|device_hostname, device_ip, user_username|
|Signal Name|Solarwinds Suspicious Child Processes|
|Summary Expression|SUNBURST backdoor indicator detected on host: {{device_hostname}}|
|Score/Severity|Static: 5|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0001, _mitreAttackTechnique:T1195, _mitreAttackTechnique:T1195.001, _mitreAttackTechnique:T1195.002|
## Vendors and Products
- [CrowdStrike - FDR](../products/569a3a44-c29f-492e-bcf4-5dc04e2ab0f3.md)
- [Microsoft - Azure](../products/a1225af5-e778-4068-a9a2-47da93d1ff24.md)
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|baseImage|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|file_path|
|Normalized Schema|parentBaseImage|
|Normalized Schema|user_username|


