# [Rules](README.md): Azure - Group Information Downloaded

## Description
Detects group information enumeration. This could be used by an adversary to learn about the environment

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Discovery|
|Apply Risk to Entities|device_hostname, device_ip, user_username, srcDevice_ip|
|Signal Name|Azure - Group Information Downloaded|
|Summary Expression|IP: {{device_ip}} successfully downloaded user information|
|Score/Severity|Static: 1|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0007, _mitreAttackTactic:TA0009, _mitreAttackTechnique:T1069, _mitreAttackTechnique:T1530, _mitreAttackTechnique:T1069.002, _mitreAttackTechnique:T1069.003|
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
|Normalized Schema|user_username|


