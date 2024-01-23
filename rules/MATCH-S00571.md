# [Rules](README.md): Sofacy Trojan Loader

## Description
Detects Trojan loader acitivty as used by APT28

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Unknown/Other|
|Apply Risk to Entities|device_hostname, user_username|
|Signal Name|Sofacy Trojan Loader|
|Summary Expression|Potential Sofacy Trojan Loader activity detected on {{device_hostname}}|
|Score/Severity|Static: 5|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0002, _mitreAttackTechnique:T1569, _mitreAttackTechnique:T1204, _mitreAttackTechnique:T1569.002, _mitreAttackTechnique:T1204.002, _mitreAttackTechnique:T1204.003|
## Vendors and Products
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|commandLine|
|Normalized Schema|device_hostname|
|Normalized Schema|user_username|


