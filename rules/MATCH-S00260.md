# [Rules](README.md): Azure - External User Invitation Redeemed

## Description
Detecets when an external user redeems an invitation to create an Azure account. This can be routine activity, but could be used as a mechanism for adversary persistence.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Initial Access|
|Apply Risk to Entities|device_hostname, device_ip, user_username, targetUser_username, srcDevice_ip|
|Signal Name|Azure - External User Invitation Redeemed|
|Summary Expression|User: {{user_username}} redeemed external user invitation from IP: {{device_ip}}|
|Score/Severity|Static: 1|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0001, _mitreAttackTechnique:T1199|
## Vendors and Products
- [Microsoft - Azure](../products/a1225af5-e778-4068-a9a2-47da93d1ff24.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|action|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|targetUser_username|
|Normalized Schema|user_username|


