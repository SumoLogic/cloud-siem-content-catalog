# [Rules](README.md): Okta API Token Created

## Description
Detect when a new Okta API token is created.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Privilege Escalation|
|Apply Risk to Entities|user_username, srcDevice_ip|
|Signal Name|Okta API Token Created|
|Summary Expression|User: {{user_username}} created new API token|
|Score/Severity|Static: 1|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0004, _mitreAttackTechnique:T1078, _mitreAttackTechnique:T1078.004, _mitreAttackTactic:TA0003, _mitreAttackTechnique:T1136, _mitreAttackTechnique:T1136.003, _mitreAttackTechnique:T1552.005, _mitreAttackTechnique:T1552|
## Vendors and Products
- [Okta - Single Sign-On](../products/51278354-d6b5-4c8e-a8fd-8197df334e67.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_vendor|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|user_username|


