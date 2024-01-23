# [Rules](README.md): Samsam Test File Write

## Description
The rule looks for a file named "test.txt" written to the windows system directory tree, which is consistent with Samsam propagation.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Execution|
|Apply Risk to Entities|device_ip, device_hostname, user_username|
|Signal Name|Samsam Test File Write|
|Summary Expression|Samsam ransomware indicator detected on host: {{device_hostname}}|
|Score/Severity|Static: 4|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0002, _mitreAttackTactic:TA0005, _mitreAttackTactic:TA0040, _mitreAttackTechnique:T1486, _mitreAttackTechnique:T1070, _mitreAttackTechnique:T1070.004, _mitreAttackTechnique:T1027, _mitreAttackTechnique:T1027.001, _mitreAttackTechnique:T1059, _mitreAttackTechnique:T1059.003|
## Vendors and Products
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|baseImage|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|file_basename|
|Normalized Schema|file_path|
|Normalized Schema|user_username|


