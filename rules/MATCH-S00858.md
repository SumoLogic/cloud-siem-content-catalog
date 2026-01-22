# [Rules](README.md): Zoom - Group Admin Added

## Description
The Group admin added event is triggered every time one of your app users or account users add a group admin.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Persistence|
|Apply Risk to Entities|user_username|
|Signal Name|Zoom - Group Admin Added - {{action}}|
|Summary Expression|User: {{user_username}} {{action}}|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0003, _mitreAttackTechnique:T1098|
## Vendors and Products
- [Zoom - Zoom](../products/ad8d40a9-ee64-4615-bd92-aa964b4ae3b0.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|action|
|Normalized Schema|metadata_vendor|
|Normalized Schema|user_username|


