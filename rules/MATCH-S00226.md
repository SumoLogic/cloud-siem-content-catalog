# [Rules](README.md): Azure - Add Member to Group

## Description
Detects a user being added to a group. This may be a routine activity, but could be indicative of an attempt to escalate account privileges. It is recommended to add additional expression logic to this rule to either exclude non-sensitive groups, or to only include sensitive groups.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Privilege Escalation|
|Apply Risk to Entities|device_hostname, device_ip, user_username, targetUser_username, srcDevice_ip|
|Signal Name|Azure - Added a Member to Group|
|Summary Expression|{{user_username}} added {{changeTarget}} to group {{fields['modified_property_Group.DisplayName']}}|
|Score/Severity|Static: 1|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0001, _mitreAttackTactic:TA0003, _mitreAttackTactic:TA0004, _mitreAttackTactic:TA0005, _mitreAttackTechnique:T1078, _mitreAttackTechnique:T1098, _mitreAttackTechnique:T1078.004, _mitreAttackTechnique:T1078.002, _mitreAttackTechnique:T1098.001, _mitreAttackTechnique:T1098.003|
## Vendors and Products
- [Microsoft - Azure](../products/a1225af5-e778-4068-a9a2-47da93d1ff24.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|changeType|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|targetUser_username|
|Normalized Schema|user_username|


