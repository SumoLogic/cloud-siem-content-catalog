# [Rules](README.md): Directory Traversal - Successful

## Description
Directory traversal is an attempt by an attacker to access files located on the host which are not intended to be returned by the web server. For example, attackers seeking usernames/passwords for the host will focus on paths like ../../etc/passwd, ../../../etc/shadow, etc. When successful, a directory traversal attack results in the attacker gaining access to sensitive information and identifying a mechanism of future attack. When unsuccessful, directory traversal is an indication of ongoing external reconnaissance.

## Additional Details
|Detail|Value|
|----|----|
|Type|Match|
|Category|Initial Access|
|Apply Risk to Entities|device_ip, srcDevice_ip, dstDevice_ip, device_hostname, srcDevice_hostname, dstDevice_hostname|
|Signal Name|Directory Traversal - Successful|
|Summary Expression|Successful directory traversal detected from source IP: {{srcDevice_ip}}|
|Score/Severity|Static: 6|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0001, _mitreAttackTactic:TA0007, _mitreAttackTactic:TA0009, _mitreAttackTechnique:T1083, _mitreAttackTechnique:T1213, _mitreAttackTechnique:T1213.001|
## Vendors and Products
- [Amazon AWS - Application Load Balancer](../products/5bb9e0b3-8d57-4b10-8952-0b6ffe91b599.md)
- [Bro - Bro](../products/37C866BF-72E1-470A-9072-EDB908F56951.md)
- [Cloudflare - Logpush](../products/c2503fcc-ef30-4e40-bb32-0bf47151b140.md)
- [Microsoft - Azure](../products/a1225af5-e778-4068-a9a2-47da93d1ff24.md)
- [Microsoft - IIS](../products/fca8785d-4823-4442-86b2-8acbaa176da4.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|dstDevice_hostname|
|Normalized Schema|dstDevice_ip|
|Normalized Schema|dstDevice_ip_isInternal|
|Normalized Schema|http_response_statusCode|
|Normalized Schema|http_url|
|Normalized Schema|listMatches|
|Normalized Schema|srcDevice_hostname|
|Normalized Schema|srcDevice_ip|


