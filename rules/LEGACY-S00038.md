# [Rules](README.md): Fortinet High App-Risk

## Description
This signal fires when Fortinet detects a high risk application within the environment

## Additional Details
|Detail|Value|
|----|----|
|Type|Match|
|Category|Execution|
|Apply Risk to Entities|device_ip, user_username, device_hostname|
|Signal Name|Fortinet High App-Risk|
|Summary Expression|High risk application {{action}} from {{srcDevice_ip}}|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0002|
## Vendors and Products
- [Fortinet - Fortigate](../products/c57e2c85-4fc1-4fb7-8fa1-dbc5235231ad.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|severity|
|Normalized Schema|user_username|


