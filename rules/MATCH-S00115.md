# [Rules](README.md): G Suite - Admin - User Settings - Turn Off 2SV

## Description
Admin disabled 2SV for user

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Persistence|
|Apply Risk to Entities|user_username|
|Signal Name|G Suite - Admin - User Settings - Turn Off 2SV - " {{user_email}}"|
|Summary Expression|User: {{user_username}} performed action: {{action}}|
|Score/Severity|Static: 2|
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
|Normalized Schema|user_email|
|Normalized Schema|user_username|


