# [Rules](README.md): G Suite - Excessive OAuth Application Permissions Scope

## Description
Alert when an OAuth application has requested a high number of permissions to aspects of G Suite.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Execution|
|Apply Risk to Entities|user_username|
|Signal Name|G Suite - Excessive OAuth Application Permissions Scope|
|Summary Expression|User: {{user_username}} set excessive OAuth permission scope on application: {{application}}|
|Score/Severity|Static: 2|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0002, _mitreAttackTactic:TA0005, _mitreAttackTactic:TA0008, _mitreAttackTechnique:T1550, _mitreAttackTechnique:T1550.001|
## Vendors and Products
- [Google - G Suite](../products/e73cd65a-7a4b-4ce9-9d73-e5d9c824c214.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|application|
|Direct from Record|fields['event.parameters.scope.10']|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|user_username|


