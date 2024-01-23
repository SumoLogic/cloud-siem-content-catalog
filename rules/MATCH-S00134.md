# [Rules](README.md): Windows User Account Created with Abnormal Naming Convention

## Description
'changeTarget' should be populated with a reguar expression that matches the user naming convention. This rule detects a user account that has been created that does not fit the normal naming convention established. If an unauthorized account has been created, it could be used to maliciously access additional systems.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Persistence|
|Apply Risk to Entities|device_hostname, device_ip, user_username|
|Signal Name|Windows User Account Created with Abnormal Naming Convention|
|Summary Expression|Detected unusually named account creation with name: {{targetUser_username}} on host: {{device_hostname}}|
|Score/Severity|Static: 3|
|Enabled by Default|False|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0003, _mitreAttackTechnique:T1136, _mitreAttackTechnique:T1136.001, _mitreAttackTechnique:T1136.002|
## Vendors and Products
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|user_username|


