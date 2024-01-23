# [Rules](README.md): SharPersist A Utility

## Description
From FireEye Red Team Tool Countermeasures:
This IOC detects windows persistence activity performed by the Sharpersist utility. It has multiple persistence functionalities such as Keepass, hotkey, new schedule task, Startup Folder and Scheduled Task Backdoor.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Persistence|
|Apply Risk to Entities|device_hostname, user_username|
|Signal Name|SharPersist A Utility|
|Summary Expression|None|
|Score/Severity|Static: 5|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0002, _mitreAttackTactic:TA0003, _mitreAttackTactic:TA0004, _mitreAttackTechnique:T1047, _mitreAttackTechnique:T1053, _mitreAttackTechnique:T1053.005, _mitreAttackTechnique:T1547, _mitreAttackTechnique:T1547.001|
## Vendors and Products
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|baseImage|
|Normalized Schema|commandLine|
|Normalized Schema|device_hostname|
|Normalized Schema|user_username|


