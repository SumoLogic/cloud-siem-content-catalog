# [Rules](README.md): Okta Administrator Access Granted

## Description
Detects Okta administrator access being granted. This is where policies are set, users are managed, and apps are controlled.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Privilege Escalation|
|Apply Risk to Entities|user_username, srcDevice_ip, targetUser_username|
|Signal Name|Okta Administrator Access Granted|
|Summary Expression|User: {{user_username}} granted administrative access to user: {{targetUser_username}}|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0004, _mitreAttackTechnique:T1078, _mitreAttackTechnique:T1078.004, _mitreAttackTactic:TA0003, _mitreAttackTechnique:T1136, _mitreAttackTechnique:T1136.003, _mitreAttackTechnique:T1552.005, _mitreAttackTechnique:T1552|
## Vendors and Products
- [Okta - Single Sign-On](../products/51278354-d6b5-4c8e-a8fd-8197df334e67.md)


## Fields Used

|Origin|Field|
|----|----|
|Direct from Record|fields['debugContext.debugData.privilegeGranted']|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_vendor|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|targetUser_username|
|Normalized Schema|user_username|


