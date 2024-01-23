# [Rules](README.md): Malicious Named Pipes

## Description
Observes for known pipe names associated with malicious activity

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Unknown/Other|
|Apply Risk to Entities|device_hostname, user_username|
|Signal Name|Malicious Named Pipes|
|Summary Expression|Observed potential malicious pipe with name {{resource}}  on {{device_hostname}}|
|Score/Severity|Static: 5|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0005, _mitreAttackTactic:TA0004, _mitreAttackTechnique:T1055, _mitreAttackTechnique:T1055.001, _mitreAttackTechnique:T1055.002, _mitreAttackTechnique:T1055.003, _mitreAttackTechnique:T1055.009, _mitreAttackTechnique:T1055.012|
## Vendors and Products
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|device_hostname|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|resource|
|Normalized Schema|user_username|


