# [Rules](README.md): SMB Scanning Detected

## Description
This rule looks for a host scanning other SMB hosts for specific commands similar to WannaCry

## Additional Details
|Detail|Value|
|----|----|
|Type|Threshold|
|Category|Lateral Movement|
|Apply Risk to Entities|device_hostname, device_ip, srcDevice_hostname, srcDevice_ip, user_username|
|Signal Name|SMB Scanning Detected|
|Summary Expression|SMB hosts scanned by IP: {{srcDevice_ip}}|
|Threshold Count|15|
|Threshold Window|5m|
|Score/Severity|Static: 1|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0007, _mitreAttackTactic:TA0008, _mitreAttackTactic:TA0043, _mitreAttackTechnique:T1135, _mitreAttackTechnique:T1595, _mitreAttackTechnique:T1595.001, _mitreAttackTechnique:T1021, _mitreAttackTechnique:T1021.002|
## Vendors and Products
- [Bro - Bro](../products/37C866BF-72E1-470A-9072-EDB908F56951.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|bro_smb_command.name|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|listMatches|
|Normalized Schema|srcDevice_hostname|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|user_username|


