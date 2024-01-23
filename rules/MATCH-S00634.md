# [Rules](README.md): Okta Admin App Access Attempt Failed

## Description
Detects failed access attempts to the Okta admin app. This is where policies are set, users are managed, and apps are controlled.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Privilege Escalation|
|Apply Risk to Entities|user_username, srcDevice_ip|
|Signal Name|Okta Admin App Access Attempt Failed|
|Summary Expression|User: {{user_username}} failed attempt to access Okta admin app.|
|Score/Severity|Static: 5|
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
|Normalized Schema|success|
|Normalized Schema|user_username|


