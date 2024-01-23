# [Rules](README.md): SharPersist Utility

## Description
From FireEye Red Team Tool Countermeasures:
This IOC detects a Windows Persistence Toolkit called SharPersist.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Persistence|
|Apply Risk to Entities|device_hostname, user_username|
|Signal Name|SharPersist Utility|
|Summary Expression|SharPersist Utility indicator detected on host: {{device_hostname}}|
|Score/Severity|Static: 5|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0003, _mitreAttackTactic:TA0004, _mitreAttackTechnique:T1547, _mitreAttackTechnique:T1547.001, _mitreAttackTechnique:T1053, _mitreAttackTechnique:T1053.005|
## Vendors and Products
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|commandLine|
|Normalized Schema|device_hostname|
|Normalized Schema|file_hash_md5|
|Normalized Schema|file_path|
|Normalized Schema|user_username|


