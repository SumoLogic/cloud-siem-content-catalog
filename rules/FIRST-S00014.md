# [Rules](README.md): First Seen Driver Load - Host

## Description
{{device_hostname}} loaded new driver {{file_path}}.

## Additional Details
|Detail|Value|
|----|----|
|Type|First Seen|
|Category|Execution|
|Apply Risk to Entities|device_hostname|
|Signal Name|First Seen Driver Load: {{file_path}} from Host|
|Summary Expression|{{device_hostname}} loaded new driver {{file_path}}|
|Retention Window|7776000000|
|Baseline Window|1814400000|
|Baseline Type|PER_ENTITY|
|Score/Severity|Static: 2|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0002, _mitreAttackTechnique:T1014|
## Vendors and Products
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|device_hostname|
|Normalized Schema|file_path|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|


