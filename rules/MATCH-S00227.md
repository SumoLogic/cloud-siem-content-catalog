# [Rules](README.md): G Suite - Unauthorized OAuth Application

## Description
Alert when a non-approved OAuth Application has been identified on Google G Suite. This rule is disabled by default as a list of approved OAuth applications is required to be enabled. The approved applications should be added to the rule logic under the 'application not in' condition.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Execution|
|Apply Risk to Entities|user_username|
|Signal Name|G Suite - Unauthorized OAuth Application - "{{application}}"|
|Summary Expression|Unauthorized OAuth Application: {{application}} on user: {{user_username}}|
|Score/Severity|Static: 2|
|Enabled by Default|False|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0002, _mitreAttackTactic:TA0005, _mitreAttackTactic:TA0008, _mitreAttackTechnique:T1550, _mitreAttackTechnique:T1550.001|
## Vendors and Products
- [Google - G Suite](../products/e73cd65a-7a4b-4ce9-9d73-e5d9c824c214.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|application|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|user_username|


