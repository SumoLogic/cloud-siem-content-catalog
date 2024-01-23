# [Rules](README.md): Registry Modification - Windows Logon Script

## Description
Logon scripts are executed on user logon and can be used to establish persistence. This detection requires registry monitoring.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Unknown/Other|
|Apply Risk to Entities|device_hostname|
|Signal Name|Registry Modification - Windows Logon Script|
|Summary Expression|Windows Logon Script modification detected on host: {{device_hostname}}|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0003, _mitreAttackTechnique:T1037, _mitreAttackTechnique:T1037.001|
## Vendors and Products
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|device_hostname|


