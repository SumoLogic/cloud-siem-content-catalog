# [Rules](README.md): OneLogin - API Credentials - New Key Created

## Description
Detects creation of API Keys. API Keys should be closely monitored to prevent unauthorized access.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Unknown/Other|
|Apply Risk to Entities|device_hostname, device_ip, user_username|
|Signal Name|OneLogin - API Credentials - New Key Created|
|Summary Expression|User: {{user_username}} created new API credential key|
|Score/Severity|Static: 1|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0002, _mitreAttackTechnique:T1106, _mitreAttackTechnique:T1552.005, _mitreAttackTechnique:T1552|
## Vendors and Products
- [OneLogin - OneLogin Single Sign-On](../products/e43ba0e4-1e3f-40c6-8bca-cb06a656a40b.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_vendor|
|Normalized Schema|user_username|


