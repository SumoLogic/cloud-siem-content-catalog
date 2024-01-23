# [Rules](README.md): Registry Modification - Authentication Package

## Description
Malicious authentication packages can be added via the Windows Registry. This rule requires registry monitoring to be setup on the endpoint.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Persistence|
|Apply Risk to Entities|device_hostname|
|Signal Name|Registry Modification - Authentication Package|
|Summary Expression|LSA Authentication package: {{resource}} added on host: {{device_hostname}}|
|Score/Severity|Static: 5|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTechnique:T1547.002, _mitreAttackTactic:TA0003, _mitreAttackTechnique:T1547, _mitreAttackTechnique:T1556.002|
## Vendors and Products
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|changeTarget|
|Normalized Schema|device_hostname|


