# [Rules](README.md): Windows - User Adds Self to Security Group

## Description
A user adding themselves to a security group may indicate the attempt to escalate their privileges

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Privilege Escalation|
|Apply Risk to Entities|device_hostname, device_ip, user_username|
|Signal Name|Windows - User Adds Self to Security Group|
|Summary Expression|The user account {{user_username}} has added themselves to the Windows security group {{changeTarget}}|
|Score/Severity|Static: 5|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0005, _mitreAttackTactic:TA0004, _mitreAttackTechnique:T1484, _mitreAttackTechnique:T1484.001|
## Vendors and Products
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Direct from Record|fields['EventData.MemberSid']|
|Direct from Record|fields['EventData.SubjectUserSid']|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|user_username|


