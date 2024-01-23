# [Rules](README.md): G Suite - Login - Government Attack Warning

## Description
Government-backed attack warnings

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Initial Access|
|Apply Risk to Entities|user_username, srcDevice_ip|
|Signal Name|G Suite - Login - Government Attack Warning|
|Summary Expression|Government-backed attack warning from IP: {{srcDevice_ip}} on user: {{user_username}}|
|Score/Severity|Static: 4|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0001, _mitreAttackTactic:TA0003, _mitreAttackTactic:TA0004, _mitreAttackTactic:TA0005, _mitreAttackTechnique:T1078, _mitreAttackTechnique:T1078.004|
## Vendors and Products
- [Google - G Suite](../products/e73cd65a-7a4b-4ce9-9d73-e5d9c824c214.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|user_username|


