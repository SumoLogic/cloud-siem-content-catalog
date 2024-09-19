# [Rules](README.md): LNKSmasher Utility Commands

## Description
From FireEye Red Team Tool Countermeasures:
LNKSmasher embeds an arbitrary payload in an LNK that can be executed by the embedded command. This IOC will detect the commands executed by both the new and old version of LNKSmasher.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Execution|
|Apply Risk to Entities|device_hostname, user_username|
|Signal Name|LNKSmasher Utility Commands|
|Summary Expression|Command with LNKSmasher Utility indicators detected on host: {{device_hostname}}|
|Score/Severity|Static: 5|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0002, _mitreAttackTactic:TA0005, _mitreAttackTechnique:T1202|
## Vendors and Products
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|commandLine|
|Normalized Schema|device_hostname|
|Normalized Schema|user_username|


