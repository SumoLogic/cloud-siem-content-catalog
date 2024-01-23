# [Rules](README.md): User Account Created and Deleted in 24 Hours

## Description
User Account Created and Deleted in 24 Hours. The temporary existence of a user account may be suspicious activity.

## Additional Details
|Detail|Value|
|----|----|
|Type|Threshold|
|Category|Privilege Escalation|
|Apply Risk to Entities|device_hostname, device_ip, user_username|
|Signal Name|User Account Created and Deleted in 24 Hours|
|Summary Expression|User account: {{changeTarget}} create and deleted within 24 hours|
|Threshold Count|2|
|Threshold Window|24h|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0003, _mitreAttackTactic:TA0004, _mitreAttackTactic:TA0040, _mitreAttackTechnique:T1098, _mitreAttackTechnique:T1098.001, _mitreAttackTechnique:T1098.002, _mitreAttackTechnique:T1098.003, _mitreAttackTechnique:T1136, _mitreAttackTechnique:T1136.001, _mitreAttackTechnique:T1136.002, _mitreAttackTechnique:T1531|
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


