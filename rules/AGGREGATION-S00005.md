# [Rules](README.md): Suspicious System Enumeration Occurring in Quick Succession

## Description
Threat actors will attempt to enuerate various system settings in order to explore privilige escalation avenues or to locate potentially sensitive data.

## Additional Details
|Detail|Value|
|----|----|
|Type|Aggregation|
|Category|Discovery|
|Apply Risk to Entities|device_hostname|
|Signal Name|Suspicious System Enumeration Occurring in Quick Succession|
|Summary Expression|{{device_hostname}} has recorded a number of system enumeration commands issued in rapid sucession, indicating a potentially malicious system enumeration attempt.|
|Aggregation Window|10m|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0043, _mitreAttackTechnique:T1589, _mitreAttackTechnique:T1592, _mitreAttackTechnique:T1590.005, _mitreAttackTechnique:T1590.002, _mitreAttackTechnique:T1590.001|
## Vendors and Products
- [CrowdStrike - FDR](../products/569a3a44-c29f-492e-bcf4-5dc04e2ab0f3.md)
- [Microsoft - Azure](../products/a1225af5-e778-4068-a9a2-47da93d1ff24.md)
- [Microsoft - Defender Advanced Hunting](../products/3382523e-2072-41bd-b50b-6b148957d0b0.md)
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|cmd_count|
|Normalized Schema|commandLine|
|Normalized Schema|device_hostname|
|Normalized Schema|file_path|
|Normalized Schema|listMatches|
|Normalized Schema|lower|
|Normalized Schema|parentBaseImage|


