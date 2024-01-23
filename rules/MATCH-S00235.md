# [Rules](README.md): Azure - Create User

## Description
Detects user creation. While this is a routine activity, user creation could be used by an adversary for persistence.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Persistence|
|Apply Risk to Entities|device_hostname, device_ip, targetUser_username, user_username, srcDevice_ip|
|Signal Name|Azure - User Created|
|Summary Expression|User {{targetUser_username}} created from IP {{srcDevice_ip}} by {{user_username}}|
|Score/Severity|Static: 1|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0003, _mitreAttackTechnique:T1136, _mitreAttackTechnique:T1136.002, _mitreAttackTechnique:T1136.003|
## Vendors and Products
- [Microsoft - Azure](../products/a1225af5-e778-4068-a9a2-47da93d1ff24.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|action|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|success|
|Normalized Schema|targetUser_username|
|Normalized Schema|user_username|


