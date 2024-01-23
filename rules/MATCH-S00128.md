# [Rules](README.md): G Suite - Login - Account Warning

## Description
Google Accounts warnings

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Initial Access|
|Apply Risk to Entities|user_username, srcDevice_ip|
|Signal Name|G Suite - Login - Account Warning - {{action}}|
|Summary Expression|Account Warning for source IP {{srcDevice_ip}} with action: {{action}}|
|Score/Severity|Static: 2|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0001, _mitreAttackTactic:TA0003, _mitreAttackTactic:TA0004, _mitreAttackTactic:TA0005, _mitreAttackTactic:TA0006, _mitreAttackTactic:TA0042, _mitreAttackTechnique:T1078, _mitreAttackTechnique:T1078.004, _mitreAttackTechnique:T1586, _mitreAttackTechnique:T1586.002|
## Vendors and Products
- [Google - G Suite](../products/e73cd65a-7a4b-4ce9-9d73-e5d9c824c214.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|action|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|user_username|


