# [Rules](README.md): Solarwinds Suspicious URL Hostname

## Description
From FireEye Red Team Tool Countermeasures: This rule identifies URL requests mimicking SolarWinds network traffic, to non-SolarWinds domains. This rule will only match on instances where communication does not occur over SSL/TLS. These requests may be evidence of the SUNBURST backdoor. SUNBURST is a backdoor that has the ability to spawn and kill processes, write and delete files, set and create registry keys, gather system information, and disable a set of forensic analysis tools and services.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Initial Access|
|Apply Risk to Entities|device_hostname, device_ip, srcDevice_hostname, srcDevice_ip, user_username|
|Signal Name|Solarwinds Suspicious URL Hostname|
|Summary Expression|Solarwinds suspicious URL visited on host: {{device_hostname}}|
|Score/Severity|Static: 5|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0001, _mitreAttackTechnique:T1195, _mitreAttackTechnique:T1195.001, _mitreAttackTechnique:T1195.002|
## Vendors and Products
- [Bro - Bro](../products/37C866BF-72E1-470A-9072-EDB908F56951.md)
- [Fortinet - Fortigate](../products/c57e2c85-4fc1-4fb7-8fa1-dbc5235231ad.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|http_hostname|
|Normalized Schema|http_url|
|Normalized Schema|http_url_rootDomain|
|Normalized Schema|lower|
|Normalized Schema|srcDevice_hostname|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|user_username|


