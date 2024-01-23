# [Rules](README.md): Azure - Add Member to Role Outside of PIM

## Description
Privileged Identity Management (PIM) allows administrators to provide users privileged access with greater oversight of activties undertaken  while said access is granted as well as control over the duration of access.

Adding a user to a role, especially one with administrative privileges, outside of PIM may indicate a threat actor attempting to persist privileged access.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Privilege Escalation|
|Apply Risk to Entities|device_hostname, device_ip, user_username, targetUser_username, srcDevice_ip|
|Signal Name|Azure -  Added to Role (Non-PIM)|
|Summary Expression|{{device_ip}} added {{changeTarget}} to {{fields['properties.targetResources.1.modifiedProperties.2.newValue']}}|
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
|Direct from Record|fields['identity']|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|targetUser_username|
|Normalized Schema|user_username|


