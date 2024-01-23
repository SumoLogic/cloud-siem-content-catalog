# [Rules](README.md): Backdoor.HTTP.BEACON.[Yelp Request]

## Description
From FireEye Red Team Tool Countermeasures:
Network detection rule that looks for specific HTTP header for either a POST or GET request. These are related to the HTTP request content designated within the Cobalt Strike malleable C2 profile.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Command and Control|
|Apply Risk to Entities|device_ip, device_hostname, srcDevice_hostname, srcDevice_ip, user_username|
|Signal Name|Backdoor.HTTP.BEACON.[Yelp Request]|
|Summary Expression|Suspicious HTTP Request Headers to URL: {{http_url}} on destination host: {{dstDevice_ip}}|
|Score/Severity|Static: 5|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0011, _mitreAttackTechnique:T1071, _mitreAttackTechnique:T1071.001|
## Vendors and Products
- [Bro - Bro](../products/37C866BF-72E1-470A-9072-EDB908F56951.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|bro_http_request_headers['COOKIE']|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|http_requestHeaders['COOKIE']|
|Normalized Schema|objectType|
|Normalized Schema|srcDevice_hostname|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|user_username|


