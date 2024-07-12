# [Rules](README.md): Too many empty/refused DNS queries

## Description
The DNS request/response was empty or refused. This may be an indication of DNS tunneling. (Excludes IPv4/IPv6 multicast DNS and LLMNR traffic).

## Additional Details
|Detail|Value|
|----|----|
|Type|Threshold|
|Category|Command and Control|
|Apply Risk to Entities|device_hostname, device_ip, srcDevice_hostname, srcDevice_ip, user_username|
|Signal Name|Too many empty/refused DNS queries|
|Summary Expression|Multiple empty or refused DNS requests/responses from IP {{srcDevice_ip}}|
|Threshold Count|50|
|Threshold Window|5m|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0011, _mitreAttackTechnique:T1572, _mitreAttackTechnique:T1071.004, _mitreAttackTechnique:T1071|
## Vendors and Products
- [Bro - Bro](../products/37C866BF-72E1-470A-9072-EDB908F56951.md)
- [Microsoft - DNS](../products/e362ae18-9af1-496d-9ace-efa05a8381c6.md)
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|dns_query|
|Normalized Schema|dns_returnCode|
|Normalized Schema|dstDevice_ip|
|Normalized Schema|listMatches|
|Normalized Schema|srcDevice_hostname|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|user_username|


