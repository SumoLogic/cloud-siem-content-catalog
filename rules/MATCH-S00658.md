# [Rules](README.md): Container Management Utility in Container

## Description
Container Management Utility in Container

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Execution|
|Apply Risk to Entities|user_username|
|Signal Name|Container Management Utility in Container|
|Summary Expression|User: {{user_username}} executed a container management command within the container using kubectl|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTechnique:T1609, _mitreAttackTactic:TA0002|
## Vendors and Products


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|commandLine|
|Normalized Schema|metadata_product|
|Normalized Schema|user_username|


