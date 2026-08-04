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


