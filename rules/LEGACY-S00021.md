# [Rules](README.md): Cylance Protect - Event Severity 8

## Description
Cylance Protect event with the severity between -0.899 and -0.800

## Additional Details
|Detail|Value|
|----|----|
|Type|Match|
|Category|Persistence|
|Apply Risk to Entities|device_ip, user_username, device_hostname|
|Signal Name|Cylance Protect - Event Severity 8|
|Summary Expression|Threat: {{threat_name}} with severity: {{severity}} detected on host {{device_hostname}}|
|Score/Severity|Static: 8|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0003|
## Vendors and Products
- [Cylance - Protect](../products/60829f4a-7acb-47d1-ad23-8424fcf83dcb.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|severity|
|Normalized Schema|user_username|


