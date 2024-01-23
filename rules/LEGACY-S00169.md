# [Rules](README.md): Windows Account Added To Privileged Security Group

## Description
This signal alerts on the elevation of privileges assigned to a domain user account according to Windows Event ID 4728, 4732, and/or 4756.

## Additional Details
|Detail|Value|
|----|----|
|Type|Match|
|Category|Privilege Escalation|
|Apply Risk to Entities|device_hostname, device_ip, user_username|
|Signal Name|Windows Account Added To Privileged Security Group|
|Summary Expression|User: {{user_username}} added user: {{targetUser_username}} to privileged security group|
|Score/Severity|Static: 3|
|Enabled by Default|False|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0005, _mitreAttackTactic:TA0004, _mitreAttackTechnique:T1484, _mitreAttackTechnique:T1484.001|
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


