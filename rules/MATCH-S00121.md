# [Rules](README.md): Google Workspace - Mobile - Suspicious Activity

## Description
Google Workspace alert for mobile suspicious activity

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Initial Access|
|Apply Risk to Entities|user_username, srcDevice_ip|
|Signal Name|Google Workspace - mobile - suspicious_activity - "{{action}}"|
|Summary Expression|Suspicious mobile activity from IP: {{srcDevice_ip}} on user: {{user_username}}|
|Score/Severity|Static: 2|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0001, _mitreAttackTechnique:T1078, _mitreAttackTechnique:T1078.004|
## Vendors and Products
- [Google - Google Workspace](../products/e73cd65a-7a4b-4ce9-9d73-e5d9c824c214.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|action|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|user_username|


