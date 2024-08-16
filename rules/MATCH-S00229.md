# [Rules](README.md): Azure - Member Added to Non-Global Administrator Role

## Description
Detects member additions to a non-administrative role. This is a routine activity, but could be performed by an adversary to escalate privileges.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Persistence|
|Apply Risk to Entities|device_hostname, device_ip, targetUser_username, user_username, srcDevice_ip|
|Signal Name|Azure - Member Added to {{fields['properties.targetResources.1.modifiedProperties.2.newValue']}} Role|
|Summary Expression|{{changeTarget}} added to {{fields['properties.targetResources.1.modifiedProperties.2.newValue']}} role by IP {{device_ip}}|
|Score/Severity|Static: 3|
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
|Direct from Record|fields['properties.targetResources.1.modifiedProperties.2.newValue']|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|targetUser_username|
|Normalized Schema|user_username|


