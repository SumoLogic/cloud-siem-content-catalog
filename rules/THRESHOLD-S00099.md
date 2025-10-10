# [Rules](README.md): Long URL Containing SQL Commands

## Description
Observes for long URLs with possible SQL commands within them, an indication of SQL injection activity

## Additional Details
|Detail|Value|
|----|----|
|Type|Threshold|
|Category|Execution|
|Apply Risk to Entities|device_hostname, srcDevice_hostname, dstDevice_hostname, dstDevice_ip, srcDevice_ip, device_ip|
|Signal Name|Long URL Containing SQL Commands|
|Summary Expression|SQL commands found in long URL visited from IP: {{srcDevice_ip}}|
|Threshold Count|2|
|Threshold Window|5m|
|Score/Severity|Static: 1|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0002, _mitreAttackTactic:TA0004, _mitreAttackTactic:TA0001, _mitreAttackTechnique:T1068, _mitreAttackTechnique:T1190|
## Vendors and Products
- [Amazon AWS - Application Load Balancer](../products/5bb9e0b3-8d57-4b10-8952-0b6ffe91b599.md)
- [Cisco Systems - Umbrella](../products/5ba50e74-3c05-4ea8-aeaf-5efde588c60f.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|dstDevice_hostname|
|Normalized Schema|dstDevice_ip|
|Normalized Schema|http_method|
|Normalized Schema|http_url|
|Normalized Schema|http_url_path|
|Normalized Schema|http_userAgent|
|Normalized Schema|srcDevice_hostname|
|Normalized Schema|srcDevice_ip|


