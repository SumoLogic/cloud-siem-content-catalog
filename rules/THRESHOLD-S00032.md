# [Rules](README.md): SMB Brute Force Attempt

## Description
This rule looks for failed SMB login attempts.

## Additional Details
|Detail|Value|
|----|----|
|Type|Threshold|
|Category|Lateral Movement|
|Apply Risk to Entities|device_hostname, device_ip, srcDevice_hostname, srcDevice_ip, user_username|
|Signal Name|SMB Brute Force Attempt|
|Summary Expression|Failed SMB login attempt from IP {{srcDevice_ip}}|
|Threshold Count|50|
|Threshold Window|5m|
|Score/Severity|Static: 4|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0006, _mitreAttackTactic:TA0008, _mitreAttackTechnique:T1110, _mitreAttackTechnique:T1110.001, _mitreAttackTechnique:T1110.002, _mitreAttackTechnique:T1110.003, _mitreAttackTechnique:T1110.004, _mitreAttackTechnique:T1021, _mitreAttackTechnique:T1021.002|
## Vendors and Products
- [Bro - Bro](../products/37C866BF-72E1-470A-9072-EDB908F56951.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|bro_smb_command.name|
|Normalized Schema|bro_smb_command.status|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|srcDevice_hostname|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|user_username|


