# [Rules](README.md): MS-LSAT Username Enumeration

## Description
The MS-LSAT Remote Protocol provides a number of RPC calls that can be used to map security principal SIDs to usernames. Attackers could use this technique to perform username enumeration and identify accounts on targeted systems.

## Additional Details
|Detail|Value|
|----|----|
|Type|Threshold|
|Category|Discovery|
|Apply Risk to Entities|srcDevice_ip, user_username, device_hostname, device_ip|
|Signal Name|MS-LSAT Username Enumeration|
|Summary Expression|Username enumeration from {{srcDevice_ip}}|
|Threshold Count|150|
|Threshold Window|5m|
|Score/Severity|Static: 2|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0007, _mitreAttackTechnique:T1087, _mitreAttackTechnique:T1087.001, _mitreAttackTechnique:T1087.002, _mitreAttackTechnique:T1087.003, _mitreAttackTechnique:T1087.004|
## Vendors and Products
- [Bro - Bro](../products/37C866BF-72E1-470A-9072-EDB908F56951.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|bro_dceRpc_operation|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_product|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|user_username|


