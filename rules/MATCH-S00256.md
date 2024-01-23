# [Rules](README.md): Azure - External User Invited

## Description
Detects an invitation being created for an external use to create an Azure account. This may be routine activity, but could be used as a vector for an adversary to gain access or persistence.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Initial Access|
|Apply Risk to Entities|device_hostname, device_ip, targetUser_username, user_username, srcDevice_ip|
|Signal Name|Azure - External User Invited|
|Summary Expression|User {{user_username}}  invited an external user to create an account from IP {{device_ip}}|
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


