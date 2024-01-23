# [Rules](README.md): Okta User Attempted to Access Unauthorized App

## Description
Detect when an Okta user is denied access to an app.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Privilege Escalation|
|Apply Risk to Entities|user_username, srcDevice_ip|
|Signal Name|Okta User Attempted to Access Unauthorized App|
|Summary Expression|User: {{user_username}} failed attempt to access an app.|
|Score/Severity|Static: 1|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0004, _mitreAttackTechnique:T1078, _mitreAttackTechnique:T1078.004, _mitreAttackTechnique:T1552.005, _mitreAttackTechnique:T1552|
## Vendors and Products
- [Okta - Single Sign-On](../products/51278354-d6b5-4c8e-a8fd-8197df334e67.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_vendor|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|user_username|


