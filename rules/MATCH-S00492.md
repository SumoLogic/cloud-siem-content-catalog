# [Rules](README.md): Backdoor.HTTP.GORAT.[SID1]

## Description
From FireEye Red Team Tool Countermeasures: GORAT is the modular backdoor portion of the REDFLARE framework. This rule looks for unique content within the HTTP request communications of the backdoor.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Command and Control|
|Apply Risk to Entities|device_hostname, device_ip, srcDevice_hostname, srcDevice_ip, user_username|
|Signal Name|Backdoor.HTTP.GORAT.[SID1]|
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
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|http_method|
|Normalized Schema|http_requestHeaders['ACCEPT']|
|Normalized Schema|http_requestHeaders['COOKIE']|
|Normalized Schema|http_requestHeaders['REFERER']|
|Normalized Schema|objectType|
|Normalized Schema|srcDevice_hostname|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|user_username|


