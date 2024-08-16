# [Rules](README.md): Azure - Member Added to Global Administrator Role

## Description
Detects member additions to the Global Administrator role outside of Privileged Identity Manager (PIM). This is a suspicious activity, and could be performed by an adversary to escalate privileges.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Privilege Escalation|
|Apply Risk to Entities|device_hostname, device_ip, targetUser_username, user_username, srcDevice_ip|
|Signal Name|Azure - Member Added to Global Administrator Role|
|Summary Expression|{{changeTarget}} added to Global Administrator role by IP {{device_ip}}|
|Score/Severity|Static: 4|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0003, _mitreAttackTactic:TA0004, _mitreAttackTechnique:T1098, _mitreAttackTechnique:T1098.001, _mitreAttackTechnique:T1098.002|
## Vendors and Products
- [Microsoft - Azure](../products/a1225af5-e778-4068-a9a2-47da93d1ff24.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|action|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Direct from Record|fields['modified_property_Role.DisplayName']|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|targetUser_username|
|Normalized Schema|user_username|


