# [Rules](README.md): First Seen PowerShell Execution from Computer

## Description
Observes for an Endpoint utilizing PowerShell for the first time.

## Additional Details
|Detail|Value|
|----|----|
|Type|First Seen|
|Category|Execution|
|Apply Risk to Entities|device_hostname|
|Signal Name|First Seen PowerShell Execution from Computer|
|Summary Expression|First Seen use of PowerShell executable: {{baseImage}} on the host: {{device_hostname}}|
|Retention Window|7776000000|
|Baseline Window|3024000000|
|Baseline Type|GLOBAL|
|Score/Severity|Static: 2|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0002, _mitreAttackTechnique:T1059, _mitreAttackTechnique:T1059.001|
## Vendors and Products
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|device_hostname|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|


