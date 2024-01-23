# [Rules](README.md): Request to Anomalous Web Server Software

## Description
Attackers often stage content during intrusions using external web infrastructure to host exploits, malware and other tooling. In rare cases attacker playbooks show the threat actor hosting web files by serving them using the SimpleHTTPServer server, a lightweight built-in web server module installed with Python. Occurrences of clients connecting to servers implemented using SimpleHTTPServer are anomalous and may indicate an active attack.

## Additional Details
|Detail|Value|
|----|----|
|Type|Match|
|Category|Initial Access|
|Apply Risk to Entities|device_hostname, device_ip, srcDevice_hostname, srcDevice_ip, user_username|
|Signal Name|Request to Anomalous Web Server Software|
|Summary Expression|Connection from {{srcDevice_ip}} to external anomolous web host {{dstDevice_ip}}|
|Score/Severity|Static: 2|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0001, _mitreAttackTactic:TA0011, _mitreAttackTechnique:T1102, _mitreAttackTechnique:T1102.002, _mitreAttackTechnique:T1102.003|
## Vendors and Products
- [Bro - Bro](../products/37C866BF-72E1-470A-9072-EDB908F56951.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|bro_http_response_headers['SERVER']|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|dstDevice_ip_isInternal|
|Normalized Schema|listMatches|
|Normalized Schema|srcDevice_hostname|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|user_username|


