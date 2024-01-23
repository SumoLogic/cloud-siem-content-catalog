# [Rules](README.md): Azure - Anonymous Blob Access

## Description
Detects successful anonymous blob access. This should only occur if a blob container has anonymous read access enabled, which is disabled by default. This could indicate a misconfiguration which may lead to data theft.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Collection|
|Apply Risk to Entities|srcDevice_ip|
|Signal Name|Azure - Anonymous Blob Access|
|Summary Expression|Successful anonymous blob access from IP: {{srcDevice_ip}} resource: {{resource}}|
|Score/Severity|Static: 1|
|Enabled by Default|False|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0009, _mitreAttackTechnique:T1530, _mitreAttackTechnique:T1619|
## Vendors and Products
- [Microsoft - Azure Storage Analytics](../products/4411adbb-f3f4-4e6e-a174-694fef8d7a47.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|action|
|Direct from Record|fields['request-status']|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|srcDevice_ip|


