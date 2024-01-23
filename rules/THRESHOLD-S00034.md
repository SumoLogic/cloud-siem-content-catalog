# [Rules](README.md): SSH Authentication Failures

## Description
Many SSH authentication failures from the same source IP in a short period of time can signal a brute-force attack.

## Additional Details
|Detail|Value|
|----|----|
|Type|Threshold|
|Category|Credential Access|
|Apply Risk to Entities|device_hostname, device_ip, srcDevice_hostname, srcDevice_ip, user_username|
|Signal Name|SSH Authentication Failures|
|Summary Expression|Multiple SSH authentication failures from IP: {{srcDevice_ip}}|
|Threshold Count|15|
|Threshold Window|5m|
|Score/Severity|Static: 2|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0006, _mitreAttackTechnique:T1110, _mitreAttackTechnique:T1110.001, _mitreAttackTechnique:T1110.002, _mitreAttackTechnique:T1110.003, _mitreAttackTechnique:T1110.004, _mitreAttackTactic:TA0008, _mitreAttackTechnique:T1021, _mitreAttackTechnique:T1021.004|
## Vendors and Products
- [Bro - Bro](../products/37C866BF-72E1-470A-9072-EDB908F56951.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|bro_ssh_authSuccess|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|dstDevice_ip_isInternal|
|Normalized Schema|listMatches|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_product|
|Normalized Schema|srcDevice_hostname|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|user_username|


