# [Rules](README.md): SSL Heartbleed Attack

## Description
SSL Heartbleed Attack detected

## Additional Details
|Detail|Value|
|----|----|
|Type|Match|
|Category|Credential Access|
|Apply Risk to Entities|device_hostname, device_ip, srcDevice_hostname, srcDevice_ip, user_username|
|Signal Name|SSL Heartbleed Attack|
|Summary Expression|Heartbleed attack from IP: {{srcDevice_ip}} to IP: {{dstDevice_ip}} detected|
|Score/Severity|Static: 4|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0042, _mitreAttackTechnique:T1608, _mitreAttackTechnique:T1608.003|
## Vendors and Products
- [Bro - Bro](../products/37C866BF-72E1-470A-9072-EDB908F56951.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|listMatches|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_product|
|Normalized Schema|srcDevice_hostname|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|threat_name|
|Normalized Schema|user_username|


