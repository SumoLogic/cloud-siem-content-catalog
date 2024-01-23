# [Rules](README.md): Likely doublepulsar Infected

## Description
Hosts infected with the Doublepulsar typically exhibit this type of SMB behavior

## Additional Details
|Detail|Value|
|----|----|
|Type|Match|
|Category|Defense Evasion|
|Apply Risk to Entities|srcDevice_ip, user_username, device_hostname, device_ip|
|Signal Name|Likely doublepulsar Infected|
|Summary Expression|Doublepulsar behavior detected from IP: {{srcDevice_ip}}|
|Score/Severity|Static: 8|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0005, _mitreAttackTactic:TA0008, _mitreAttackTechnique:T1210|
## Vendors and Products
- [Bro - Bro](../products/37C866BF-72E1-470A-9072-EDB908F56951.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|bro_smb_command.name|
|Normalized Schema|bro_smb_command.status|
|Normalized Schema|bro_smb_command.subCommand|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|listMatches|
|Normalized Schema|metadata_product|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|user_username|


