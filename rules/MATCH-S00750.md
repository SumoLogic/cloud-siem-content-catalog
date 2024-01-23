# [Rules](README.md): Modification of Windows Network Logon Scripts

## Description
Detects modifications of Windows Network Logon Scripts on domain controllers. Windows Network Logon Scripts are distributed to systems on a domain and can be used by an adversary to establish persistence across a network.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Persistence|
|Apply Risk to Entities|device_hostname|
|Signal Name|Modification of Windows Logon Scripts|
|Summary Expression|Observed network logon script modification on host: {{device_hostname}}|
|Score/Severity|Static: 2|
|Enabled by Default|True|
|Prototype|True|
|Tags|_mitreAttackTactic:TA0003, _mitreAttackTechnique:T1037.003, _mitreAttackTechnique:T1037|
## Vendors and Products
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|changeTarget|
|Normalized Schema|device_hostname|


