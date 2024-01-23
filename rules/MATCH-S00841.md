# [Rules](README.md): Suspicious AWS CLI Keys Access on Linux Host

## Description
Linux endpoints are often used to manage cloud resources. As a result, various keys and secrets material can often be found on file systems. Threat actors may attempt to download or view such credential material in order to access cloud resources.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Credential Access|
|Apply Risk to Entities|baseImage|
|Signal Name|Suspicious AWS CLI Keys Access on Linux Host|
|Summary Expression|AWS CLI Keys were accessed on a host by {{baseImage}}|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|True|
|Tags|_mitreAttackTactic:TA0006, _mitreAttackTechnique:T1552, _mitreAttackTechnique:T1552.001|
## Vendors and Products
- [Laurel - Laurel Linux Audit](../products/f3803323-e4d1-4098-96c6-12e5bf2ab1f5.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|baseImage|
|Normalized Schema|matches|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_vendor|


