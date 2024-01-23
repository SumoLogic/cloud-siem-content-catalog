# [Rules](README.md): Backdoor.HTTP.BEACON.[CSBundle MSOffice GET]

## Description
From FireEye Red Team Tool Countermeasures: Network detection rule that looks for a specific HTTP URI value in combination with HTTP header values and payload content. These are related to the HTTP GET request values designated within the Cobalt Strike malleable C2 profile.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Command and Control|
|Apply Risk to Entities|device_hostname, device_ip, srcDevice_hostname, srcDevice_ip, user_username|
|Signal Name|Backdoor.HTTP.BEACON.[CSBundle MSOffice GET]|
|Summary Expression|HTTP GET to {{http_url_path}} on destination host: {{dstDevice_ip}}|
|Score/Severity|Static: 5|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0011, _mitreAttackTechnique:T1071, _mitreAttackTechnique:T1071.001|
## Vendors and Products
- [Bro - Bro](../products/37C866BF-72E1-470A-9072-EDB908F56951.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|bro_http_request_headers['ACCEPT']|
|Normalized Schema|bro_http_request_headers['ACCEPT-ENCODING']|
|Normalized Schema|bro_http_request_headers['ACCEPT-LANGUAGE']|
|Normalized Schema|bro_http_request_headers['SET-COOKIE']|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|http_method|
|Normalized Schema|http_url_path|
|Normalized Schema|objectType|
|Normalized Schema|srcDevice_hostname|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|user_username|


