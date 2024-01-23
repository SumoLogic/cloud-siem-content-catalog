# [Rules](README.md): Backdoor.HTTP.BEACON.[CSBundle NYTIMES Server]

## Description
From FireEye Red Team Tool Countermeasures:

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Command and Control|
|Apply Risk to Entities|device_ip, device_hostname, srcDevice_hostname, srcDevice_ip, user_username|
|Signal Name|Backdoor.HTTP.BEACON.[CSBundle NYTIMES Server]|
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
|Normalized Schema|bro_http_response_headers['AGE']|
|Normalized Schema|bro_http_response_headers['CACHE-CONTROL']|
|Normalized Schema|bro_http_response_headers['CONTENT-ENCODING']|
|Normalized Schema|bro_http_response_headers['CONTENT-LENGTH']|
|Normalized Schema|bro_http_response_headers['CONTENT-TYPE']|
|Normalized Schema|bro_http_response_headers['SERVER']|
|Normalized Schema|bro_http_response_headers['VARY']|
|Normalized Schema|bro_http_response_headers['X-API-VERSION']|
|Normalized Schema|bro_http_response_headers['X-CACHE']|
|Normalized Schema|bro_http_response_headers['X-FIREFOX-SPDY']|
|Normalized Schema|bro_http_response_headers['X-NYT-ROUTE']|
|Normalized Schema|bro_http_response_headers['X-SERVED-BY']|
|Normalized Schema|bro_http_response_headers['X-TIMER']|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|objectType|
|Normalized Schema|srcDevice_hostname|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|user_username|


