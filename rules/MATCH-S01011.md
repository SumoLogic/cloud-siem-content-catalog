# [Rules](README.md): Threat Intel - DNS Reply Domain

## Description
This rule detects an indicator match from a threat intelligence feed

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Threat Intelligence|
|Apply Risk to Entities|srcDevice_hostname, srcDevice_ip, srcDevice_natIp, srcDevice_mac, user_username, dns_replyIp|
|Signal Name|Threat Intel - DNS Reply Domain|
|Summary Expression|Threat Intel - DNS Reply Domain detected for: {{dns_replyDomain}}|
|Score/Severity|Static: 2|
|Enabled by Default|True|
|Prototype|False|
|Tags||
## Vendors and Products


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


