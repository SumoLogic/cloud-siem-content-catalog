# [Rules](README.md): Zoom - Group Changes

## Description
Monitors Zoom group changes for additions, removals, or updates.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Persistence|
|Apply Risk to Entities|user_username|
|Signal Name|Zoom - Group Changes - {{action}}|
|Summary Expression|User: {{user_username}} {{action}} Group: {{changeTarget}}|
|Score/Severity|Static: 1|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0003, _mitreAttackTechnique:T1098, _mitreAttackTactic:TA0040, _mitreAttackTechnique:T1531|
## Vendors and Products


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|action|
|Normalized Schema|listMatches|
|Normalized Schema|metadata_vendor|
|Normalized Schema|user_username|


