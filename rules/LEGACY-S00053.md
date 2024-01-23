# [Rules](README.md): Internal Communication on Unassigned Low Ports - Destination Match

## Description
Many ports in the 0-1023 are unassigned by the IANA.  These can be used as communication channels inside a network, as there are rarely legitimate services using these ports.

## Additional Details
|Detail|Value|
|----|----|
|Type|Match|
|Category|Command and Control|
|Apply Risk to Entities|srcDevice_ip, user_username, device_hostname, device_ip|
|Signal Name|Internal Communication on Unassigned Low Ports - Destination Match|
|Summary Expression|Internal traffic from IP: {{srcDevice_ip}} to IP: {{dstDevice_ip}} on port: {{dstPort}}|
|Score/Severity|Static: 2|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0011, _mitreAttackTechnique:T1071, _mitreAttackTechnique:T1071.001|
## Vendors and Products
- [Bro - Bro](../products/37C866BF-72E1-470A-9072-EDB908F56951.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|dstDevice_ip|
|Normalized Schema|dstDevice_ip_isInternal|
|Normalized Schema|dstPort|
|Normalized Schema|ipProtocol|
|Normalized Schema|listMatches|
|Normalized Schema|metadata_product|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|srcDevice_ip_isInternal|
|Normalized Schema|user_username|


