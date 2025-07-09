# [Rules](README.md): Hexadecimal User-Agent

## Description
User-Agent strings with hexadecimal values are often indicative of malware.

## Additional Details
|Detail|Value|
|----|----|
|Type|Match|
|Category|Command and Control|
|Apply Risk to Entities|device_ip, srcDevice_ip, dstDevice_ip, device_hostname, srcDevice_hostname, dstDevice_hostname|
|Signal Name|Hexadecimal User-Agent|
|Summary Expression|Hexadecimal detected in user-agent: {{http_userAgent}}|
|Score/Severity|Static: 2|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0010, _mitreAttackTactic:TA0011, _mitreAttackTechnique:T1132, _mitreAttackTechnique:T1132.001, _mitreAttackTactic:TA0009, _mitreAttackTechnique:T1213, _mitreAttackTechnique:T1213.001|
## Vendors and Products
- [Bro - Bro](../products/37C866BF-72E1-470A-9072-EDB908F56951.md)
- [Cloudflare - Logpush](../products/c2503fcc-ef30-4e40-bb32-0bf47151b140.md)
- [Palo Alto Networks - Next Generation Firewall](../products/46f5fa2c-1a62-4692-82ad-ed87800a0adb.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|dstDevice_hostname|
|Normalized Schema|dstDevice_ip|
|Normalized Schema|http_userAgent|
|Normalized Schema|srcDevice_hostname|
|Normalized Schema|srcDevice_ip|


