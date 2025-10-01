# [Rules](README.md): Windows Service Executed from Nonstandard Execution Path

## Description
Windows services launching from locations outside of their standard installation path is a common malware persistence mechanism.

## Additional Details
|Detail|Value|
|----|----|
|Type|Match|
|Category|Persistence|
|Apply Risk to Entities|device_hostname, device_ip, user_username|
|Signal Name|Windows Service Executed from Nonstandard Execution Path|
|Summary Expression|Detected service: {{baseImage}} execution from nonstandard path on host: {{device_hostname}}|
|Score/Severity|Static: 7|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0002, _mitreAttackTactic:TA0003, _mitreAttackTactic:TA0005, _mitreAttackTechnique:T1036, _mitreAttackTechnique:T1036.003, _mitreAttackTechnique:T1036.004, _mitreAttackTechnique:T1036.005, _mitreAttackTechnique:T1569, _mitreAttackTechnique:T1569.002|
## Vendors and Products
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)
- [VMware - Carbon Black Cloud](../products/f9cea291-9030-4e41-9836-6dd9274d6df4.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|baseImage|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|lower|
|Normalized Schema|user_username|


