# [Rules](README.md): Backdoor.HTTP.BEACON.[CSBundle USAToday Server]

## Description
From FireEye Red Team Tool Countermeasures: Network detection rule that looks for specific response body content within Cobalt Strike malleable C2 profile. This is used as an attempt to blend in and provide legitimacy within the malware C2 communications.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Command and Control|
|Apply Risk to Entities|device_hostname, device_ip, srcDevice_hostname, srcDevice_ip, user_username|
|Signal Name|Backdoor.HTTP.BEACON.[CSBundle USAToday Server]|
|Summary Expression|Suspicious HTTP Response Headers from URL: {{http_url}} on destination host: {{dstDevice_ip}}|
|Score/Severity|Static: 5|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0011, _mitreAttackTechnique:T1071, _mitreAttackTechnique:T1071.001|
## Vendors and Products
- [Bro - Bro](../products/37C866BF-72E1-470A-9072-EDB908F56951.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|bro_http_response_headers['ACCEPT-RANGES']|
|Normalized Schema|bro_http_response_headers['CACHE-CONTROL']|
|Normalized Schema|bro_http_response_headers['CONNECTION']|
|Normalized Schema|bro_http_response_headers['CONTENT-SECURITY-POLICY']|
|Normalized Schema|bro_http_response_headers['CONTENT-TYPE']|
|Normalized Schema|bro_http_response_headers['STRICT-TRANSPORT-SECURITY']|
|Normalized Schema|bro_http_response_headers['VARY']|
|Normalized Schema|bro_http_response_headers['X-CACHE']|
|Normalized Schema|bro_http_response_headers['X-TIMER']|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|objectType|
|Normalized Schema|srcDevice_hostname|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|user_username|


