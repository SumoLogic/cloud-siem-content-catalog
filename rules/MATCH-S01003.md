# [Rules](README.md): Threat Intel - SHA1 Match

## Description
This rule detects a SHA1 hash indicator match from a threat intelligence feed

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Threat Intelligence|
|Apply Risk to Entities|device_hostname, srcDevice_hostname, device_ip, device_natIp, srcDevice_ip, srcDevice_natIp, device_mac, srcDevice_mac, user_username, dns_replyIp|
|Signal Name|Threat Intel - File Hash Match|
|Summary Expression|The record contains a matching SHA1 hash from a threat intelligence feed: {{file_hash_sha1}}|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags||
## Vendors and Products
- [Bro - Bro](../products/37C866BF-72E1-470A-9072-EDB908F56951.md)
- [FireEye - Endpoint Security](../products/8c342fa0-4147-47c9-b574-965ad2eddafa.md)
- [Fortinet - Fortigate](../products/c57e2c85-4fc1-4fb7-8fa1-dbc5235231ad.md)
- [Microsoft - Azure](../products/a1225af5-e778-4068-a9a2-47da93d1ff24.md)
- [Microsoft - Defender Advanced Hunting](../products/3382523e-2072-41bd-b50b-6b148957d0b0.md)
- [Microsoft - Office 365](../products/d3ed003d-5ddd-4c7a-bea5-63eae6311833.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|SHA-1|
|Normalized Schema|confidence|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|device_mac|
|Normalized Schema|device_natIp|
|Normalized Schema|dns_replyIp|
|Normalized Schema|srcDevice_hostname|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|srcDevice_mac|
|Normalized Schema|srcDevice_natIp|
|Normalized Schema|type|
|Normalized Schema|user_username|


