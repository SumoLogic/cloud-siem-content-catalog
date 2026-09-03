# [Rules](README.md): Normalized Network Detection

## Description
Passes through a network, NDR, or WAF detection (e.g. Kemp, Palo Alto, FortiGate, FireEye, Vectra, Claroty) and adjusts the severity accordingly based on the severity provided in the log.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Command and Control|
|Apply Risk to Entities|srcDevice_ip, dstDevice_ip, srcDevice_hostname, dstDevice_hostname, http_url_fqdn, http_url|
|Signal Name|{{metadata_vendor}} {{metadata_product}} - {{threat_signalName}}|
|Summary Expression|Network detection: {{threat_signalName}} from {{srcDevice_ip}}|
|Score/Severity|None|
|Enabled by Default|True|
|Prototype|False|
|Tags||
## Vendors and Products
- [Kemp - LoadMaster](../products/e0763d80-29ce-43a0-b0ab-69c621abb3eb.md)
- [Palo Alto Networks - Next Generation Firewall](../products/46f5fa2c-1a62-4692-82ad-ed87800a0adb.md)
- [Vectra - Vectra AI](../products/d4a9e7ce-082e-4f41-891f-4c43e604c850.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|dstDevice_hostname|
|Normalized Schema|dstDevice_ip|
|Normalized Schema|http_url|
|Normalized Schema|http_url_fqdn|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|normalizedSeverity|
|Normalized Schema|srcDevice_hostname|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|threat_ruleType|
|Normalized Schema|threat_signalName|


