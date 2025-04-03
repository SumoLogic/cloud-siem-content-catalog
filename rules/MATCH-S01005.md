# [Rules](README.md): Threat Intel - Source Hostname

## Description
This rule detects an indicator match from a threat intelligence feed

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Threat Intelligence|
|Apply Risk to Entities|srcDevice_hostname, srcDevice_ip, srcDevice_natIp, srcDevice_mac, user_username, dns_replyIp|
|Signal Name|Threat Intel - Source Hostname|
|Summary Expression|Threat Intel - Source Device Hostname detected for: {{srcDevice_hostname}}|
|Score/Severity|Static: 2|
|Enabled by Default|True|
|Prototype|False|
|Tags||
## Vendors and Products
- [Cloudflare - Logpush](../products/c2503fcc-ef30-4e40-bb32-0bf47151b140.md)
- [Zscaler - Nanolog Streaming Service](../products/6299d728-14f7-455e-85c5-ea8ec65a654a.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|OR|
|Normalized Schema|confidence|
|Normalized Schema|dns_replyIp|
|Normalized Schema|listMatches|
|Normalized Schema|srcDevice_hostname|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|srcDevice_mac|
|Normalized Schema|srcDevice_natIp|
|Normalized Schema|type|
|Normalized Schema|user_username|


