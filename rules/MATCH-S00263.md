# [Rules](README.md): iOS Implant URL Pattern

## Description
Detects a string in a http request url that is associated with an iOS Implant.  

Ref: 
https://googleprojectzero.blogspot.com/2019/08/implant-teardown.html
https://twitter.com/craiu/status/1167358457344925696

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Execution|
|Apply Risk to Entities|device_hostname, device_ip, srcDevice_hostname, srcDevice_ip, user_username|
|Signal Name|iOS Implant URL Pattern|
|Summary Expression|iOS implant string detected in URL: {http_url}}|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0002, _mitreAttackTactic:TA0006, _mitreAttackTactic:TA0009, _mitreAttackTechnique:T1005, _mitreAttackTechnique:T1119, _mitreAttackTechnique:T1203, _mitreAttackTechnique:T1528|
## Vendors and Products
- [Bro - Bro](../products/37C866BF-72E1-470A-9072-EDB908F56951.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|http_url|
|Normalized Schema|srcDevice_hostname|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|user_username|


