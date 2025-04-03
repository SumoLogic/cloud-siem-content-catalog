# [Rules](README.md): Threat Intel - SSDEEP Match

## Description
This rule detects an SSDEEP hash indicator match from a threat intelligence feed

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Threat Intelligence|
|Apply Risk to Entities|device_hostname, srcDevice_hostname, device_ip, device_natIp, srcDevice_ip, srcDevice_natIp, device_mac, srcDevice_mac, user_username, dns_replyIp|
|Signal Name|Threat Intel - File Hash Match|
|Summary Expression|The record contains a matching SSDEEP hash from a threat intelligence feed: {{file_hash_ssdeep}}|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags||
## Vendors and Products


## Fields Used

|Origin|Field|
|----|----|
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


