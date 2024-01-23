# [Rules](README.md): Zoom - Account Deleted

## Description
A user account or TSP account has been deleted.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Impact|
|Apply Risk to Entities|user_username, targetUser_username|
|Signal Name|Zoom - Account Deleted - {{action}}|
|Summary Expression|User: {{user_username}} {{action}} Target User: {{targetUser_username}}|
|Score/Severity|Static: 1|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0040, _mitreAttackTechnique:T1531|
## Vendors and Products


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|action|
|Normalized Schema|listMatches|
|Normalized Schema|metadata_vendor|
|Normalized Schema|targetUser_username|
|Normalized Schema|user_username|


