# [Rules](README.md): Possible Black Energy Command and Control

## Description
Black Energy is a botnet with HTTP based Command and Control communication

## Additional Details
|Detail|Value|
|----|----|
|Type|Match|
|Category|Command and Control|
|Apply Risk to Entities|device_ip, user_username, device_hostname, srcDevice_ip|
|Signal Name|Possible Black Energy Command and Control|
|Summary Expression|Potential Command and Control traffic to {{http_url}} from source host {{srcDevice_ip}}|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0011, _mitreAttackTechnique:T1071, _mitreAttackTechnique:T1071.001|
## Vendors and Products
- [Bro - Bro](../products/37C866BF-72E1-470A-9072-EDB908F56951.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|bro_http_request_headers['CONTENT-TYPE']|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|http_method|
|Normalized Schema|http_referer_rootDomain|
|Normalized Schema|http_url|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|user_username|


