# [Rules](README.md): Suspicious Windows ANONYMOUS LOGON Account Created

## Description
Detects the creation of suspicious accounts similar to ANONYMOUS LOGON.  These accounts could be created as a covering detection vs network type 3 logons for shared resources, such as folders or printers.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Persistence|
|Apply Risk to Entities|device_hostname, device_ip, user_username|
|Signal Name|Suspicious Windows ANONYMOUS LOGON Account Created|
|Summary Expression|User: {{user_username}} created account: {{targetUser_username}} |
|Score/Severity|Static: 1|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0003, _mitreAttackTechnique:T1136, _mitreAttackTechnique:T1136.001, _mitreAttackTechnique:T1136.002|
## Vendors and Products
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|changeTarget|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|user_username|


