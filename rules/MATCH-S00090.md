# [Rules](README.md): Sumo Logic Scheduled Searches

## Description
This rule passes through Sumo Logic CIP scheduled search hits to CSE as signals.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Unknown/Other|
|Apply Risk to Entities|device_hostname, device_ip, user_username|
|Signal Name|{{threat_name}}|
|Summary Expression|{{description}}|
|Score/Severity|None|
|Enabled by Default|True|
|Prototype|False|
|Tags||
## Vendors and Products
- [Sumo Logic - Scheduled Searches](../products/3BC43668-77AA-41E6-801E-447AE1291408.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|description|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|metadata_vendor|
|Normalized Schema|severity|
|Normalized Schema|threat_name|
|Normalized Schema|user_username|


