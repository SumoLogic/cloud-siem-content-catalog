# [Rules](README.md): Doublepulsar scan - likely not infected

## Description
Doublepulsar scans to check if the host is already infected before attempting to install the backdoor. 

## Additional Details
|Detail|Value|
|----|----|
|Type|Match|
|Category|Defense Evasion|
|Apply Risk to Entities|srcDevice_ip|
|Signal Name|Doublepulsar scan - likely not infected|
|Summary Expression|Doublepulsar scan on host: {{srcDevice_ip}}|
|Score/Severity|Static: 3|
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
|Normalized Schema|listMatches|
|Normalized Schema|srcDevice_ip|


