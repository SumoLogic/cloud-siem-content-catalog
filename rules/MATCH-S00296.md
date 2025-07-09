# [Rules](README.md): Shadow Copies Deletion Using OS Utilities

## Description
When adversaries take destructive action (e.g. encrypting files for ransomware) 'shadow copies' of the file system volumes are often destroyed in order to prevent these files from being easily recovered.  This signal indicates that a command was observed that may indicate this destructive action.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Execution|
|Apply Risk to Entities|device_hostname, device_ip, user_username|
|Signal Name|Shadow Copies Deletion Using OS Utilities|
|Summary Expression|Shadow Copy deletion detected on host: {{device_hostname}}|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0002, _mitreAttackTactic:TA0005, _mitreAttackTactic:TA0040, _mitreAttackTechnique:T1070, _mitreAttackTechnique:T1070.004, _mitreAttackTechnique:T1490|
## Vendors and Products
- [CrowdStrike - FDR](../products/569a3a44-c29f-492e-bcf4-5dc04e2ab0f3.md)
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|baseImage|
|Normalized Schema|commandLine|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|user_username|


