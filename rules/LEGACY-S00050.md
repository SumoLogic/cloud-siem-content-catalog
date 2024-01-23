# [Rules](README.md): IP Address Scan - Internal

## Description
A scan of IP addresses

## Additional Details
|Detail|Value|
|----|----|
|Type|Match|
|Category|Discovery|
|Apply Risk to Entities|srcDevice_ip, user_username, device_hostname, device_ip|
|Signal Name|IP Address Scan - Internal|
|Summary Expression|External IP scan from IP: {{srcDevice_ip}}|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0043, _mitreAttackTechnique:T1046, _mitreAttackTechnique:T1595, _mitreAttackTechnique:T1595.001|
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
|Normalized Schema|srcDevice_ip|
|Normalized Schema|srcDevice_ip_isInternal|
|Normalized Schema|threat_name|
|Normalized Schema|user_username|


