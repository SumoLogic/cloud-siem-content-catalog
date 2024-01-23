# [Rules](README.md): Seatbelt Utility

## Description
From FireEye Red Team Tool Countermeasures: Seatbelt is an open source C# project that performs a number of security oriented host-survey "safety checks" relevant from both offensive and defensive security perspectives. This IOC also detects some variations of this project namely Beltalowda and Shamwow.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Execution|
|Apply Risk to Entities|device_hostname, device_ip, user_username|
|Signal Name|Seatbelt Utility|
|Summary Expression|Seatbelt host-survery utility indicator detected on host: {{device_hostname}}|
|Score/Severity|Static: 5|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0002, _mitreAttackTechnique:T1059, _mitreAttackTechnique:T1059.003|
## Vendors and Products
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|baseImage|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|user_username|


