# [Rules](README.md): Zoom - Recording Modification

## Description
Detects one of your app users or account users permanently or temporarily deletes a cloud recording.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Impact|
|Apply Risk to Entities|user_email, targetUser_username|
|Signal Name|Zoom - Recording Modification - {{action}}|
|Summary Expression|User: {{user_username}} {{action}}|
|Score/Severity|Static: 1|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0040, _mitreAttackTechnique:T1485|
## Vendors and Products


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|action|
|Normalized Schema|metadata_vendor|
|Normalized Schema|targetUser_username|
|Normalized Schema|user_email|
|Normalized Schema|user_username|


