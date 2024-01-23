# [Rules](README.md): User Created and Quickly Deleted on Linux Machine

## Description
Attackers will sometimes create and subsequently delete user accounts to perform post-exploitation activity in an attempted counter-forensic measure.

## Additional Details
|Detail|Value|
|----|----|
|Type|Chain|
|Category|Defense Evasion|
|Apply Risk to Entities|device_hostname, user_username|
|Signal Name|User Created and Quickly Deleted on Linux Machine|
|Summary Expression|User {{user_username}} was created and deleted within 1 hour on host {{device_hostname}}|
|Score/Severity|Static: 4|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0003, _mitreAttackTactic:TA0004, _mitreAttackTactic:TA0040, _mitreAttackTechnique:T1098, _mitreAttackTechnique:T1098.001, _mitreAttackTechnique:T1098.002, _mitreAttackTechnique:T1098.003, _mitreAttackTechnique:T1136, _mitreAttackTechnique:T1136.001, _mitreAttackTechnique:T1136.002, _mitreAttackTechnique:T1531|
## Vendors and Products
- [Linux - Linux OS Syslog](../products/0e20c932-d992-4bd4-b276-c15119ca5c0b.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|device_hostname|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|user_username|


