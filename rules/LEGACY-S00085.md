# [Rules](README.md): SSL Certificate Expires Soon

## Description
A server responded on a SSL or TLS service using a certificate that will expire soon.

## Additional Details
|Detail|Value|
|----|----|
|Type|Match|
|Category|Defense Evasion|
|Apply Risk to Entities|device_hostname, device_ip, srcDevice_hostname, srcDevice_ip, user_username|
|Signal Name|SSL Certificate Expires Soon|
|Summary Expression|Server responded with SSL or TLS certificate nearing expiration from IP: {{srcDevice_ip}}|
|Score/Severity|Static: 1|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0042, _mitreAttackTechnique:T1587.003, _mitreAttackTechnique:T1587, _mitreAttackTechnique:T1608, _mitreAttackTechnique:T1608.003|
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


