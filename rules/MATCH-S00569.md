# [Rules](README.md): Registry Persistence Mechanisms

## Description
Observes for registry keys associated with persistence activity

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Unknown/Other|
|Apply Risk to Entities|device_hostname|
|Signal Name|Registry Persistence Mechanisms|
|Summary Expression|A registry key associated with threat persistence has been detected on {{device_hostname}}|
|Score/Severity|Static: 2|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0003, _mitreAttackTechnique:T1112|
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


