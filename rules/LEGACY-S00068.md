# [Rules](README.md): RDP Brute Force - Success

## Description
Hydra and Ncrack are popular tools for attempting brute force attacks to access a targeted system. In this case, a brute force attempt against an RDP server has succeeded and the attacker has gained access to the targeted system.

## Additional Details
|Detail|Value|
|----|----|
|Type|Match|
|Category|Credential Access|
|Apply Risk to Entities|device_hostname, device_ip, srcDevice_hostname, srcDevice_ip, user_username|
|Signal Name|RDP Brute Force - Success|
|Summary Expression|Successful RDP brute force attempt from IP: {{srcDevice_ip}} to IP: {{dstDevice_ip}}|
|Score/Severity|Static: 7|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0006, _mitreAttackTechnique:T1110, _mitreAttackTechnique:T1110.001, _mitreAttackTechnique:T1110.002, _mitreAttackTechnique:T1110.003, _mitreAttackTechnique:T1110.004, _mitreAttackTactic:TA0001, _mitreAttackTactic:TA0003, _mitreAttackTactic:TA0004, _mitreAttackTactic:TA0005, _mitreAttackTactic:TA0008, _mitreAttackTechnique:T1078, _mitreAttackTechnique:T1078.003, _mitreAttackTechnique:T1078.002, _mitreAttackTechnique:T1078.001, _mitreAttackTechnique:T1021.001, _mitreAttackTechnique:T1021|
## Vendors and Products
- [Bro - Bro](../products/37C866BF-72E1-470A-9072-EDB908F56951.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|bro_rdp_clientName|
|Normalized Schema|bro_rdp_cookie|
|Normalized Schema|bro_rdp_result|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|dstDevice_ip|
|Normalized Schema|srcDevice_hostname|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|user_username|


