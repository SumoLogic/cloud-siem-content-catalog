# [Rules](README.md): NotPetya Ransomware Activity

## Description
Detects NotPetya ransomware activity by identifying one of these occurring: the extracted passwords are passed back to the main module via named pipe, the file system journal of drive C is deleted or windows eventlogs are cleared using wevtutil.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Execution|
|Apply Risk to Entities|device_hostname, device_ip, user_username|
|Signal Name|NotPetya Ransomware Activity|
|Summary Expression|NotPetya ransomware activity detected on host: {{device_hostname}}|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0002, _mitreAttackTactic:TA0005, _mitreAttackTactic:TA0006, _mitreAttackTechnique:T1486, _mitreAttackTechnique:T1210, _mitreAttackTechnique:T1083, _mitreAttackTechnique:T1070, _mitreAttackTechnique:T1070.001, _mitreAttackTechnique:T1036, _mitreAttackTechnique:T1036.004, _mitreAttackTechnique:T1036.005, _mitreAttackTechnique:T1003, _mitreAttackTechnique:T1003.001, _mitreAttackTechnique:T1021, _mitreAttackTechnique:T1021.002, _mitreAttackTechnique:T1053, _mitreAttackTechnique:T1053.005, _mitreAttackTechnique:T1218, _mitreAttackTechnique:T1218.011, _mitreAttackTechnique:T1518, _mitreAttackTechnique:T1518.001, _mitreAttackTechnique:T1569, _mitreAttackTechnique:T1569.002, _mitreAttackTechnique:T1529, _mitreAttackTechnique:T1078, _mitreAttackTechnique:T1078.003, _mitreAttackTechnique:T1047|
## Vendors and Products
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|baseImage|
|Normalized Schema|commandLine|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|user_username|


