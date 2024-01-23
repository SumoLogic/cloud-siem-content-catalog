# [Rules](README.md): Zoom - Account Created

## Description
A sub account, user account, or TSP account has been created.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Persistence|
|Apply Risk to Entities|user_username, targetUser_username|
|Signal Name|Zoom - Account Created - {{action}}|
|Summary Expression|User: {{user_username}} {{action}} Target User: {{targetUser_username}}|
|Score/Severity|Static: 1|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0003, _mitreAttackTechnique:T1136|
## Vendors and Products


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|action|
|Normalized Schema|listMatches|
|Normalized Schema|metadata_vendor|
|Normalized Schema|targetUser_username|
|Normalized Schema|user_username|


