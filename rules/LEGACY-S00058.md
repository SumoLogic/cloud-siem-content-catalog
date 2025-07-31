# [Rules](README.md): Pastebin Raw URL Resource Request

## Description
Attackers will often host malicious code on pastebin.com and attempt to download their additional payloads if their initial attack is successful. They will download the post with the raw URI. Generally the malicious content hosted on Pastebin.com is quickly removed automatically by the poster setting an expire time.

## Additional Details
|Detail|Value|
|----|----|
|Type|Match|
|Category|Execution|
|Apply Risk to Entities|device_ip, user_username, device_hostname, srcDevice_ip|
|Signal Name|Pastebin Raw URL Resource Request|
|Summary Expression|Raw Pastebin request from IP: {{srcDevice_ip}} to URL: {{http_url}}|
|Score/Severity|Static: 4|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0002, _mitreAttackTactic:TA0011, _mitreAttackTechnique:T1102, _mitreAttackTechnique:T1102.002, _mitreAttackTechnique:T1102.003|
## Vendors and Products
- [Bro - Bro](../products/37C866BF-72E1-470A-9072-EDB908F56951.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|dstDevice_ip_isInternal|
|Normalized Schema|http_hostname|
|Normalized Schema|http_url_path|
|Normalized Schema|listMatches|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|user_username|


