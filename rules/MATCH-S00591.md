# [Rules](README.md): Cred Dump-Tools Named Pipes

## Description
Detects well-known credential dumping tools execution via specific named pipes

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Unknown/Other|
|Apply Risk to Entities|device_hostname, user_username|
|Signal Name|Cred Dump-Tools Named Pipes|
|Summary Expression|Observed named pipes associated with credential dumping tools on {{device_hostname}}|
|Score/Severity|Static: 5|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0006, _mitreAttackTactic:TA0008, _mitreAttackTechnique:T1003, _mitreAttackTechnique:T1003.001, _mitreAttackTechnique:T1003.005, _mitreAttackTechnique:T1570|
## Vendors and Products
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|changeTarget|
|Normalized Schema|device_hostname|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|user_username|


