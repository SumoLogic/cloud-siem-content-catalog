# [Rules](README.md): Package Management Utility in Container

## Description
Package management utilities should be considered anomalous when used inside containers as containers should be provisioned with the correct tools for the task assigned to them at the image level.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Execution|
|Apply Risk to Entities|user_username|
|Signal Name|Package Management Utility in Container|
|Summary Expression|Package management software keyword found in command|
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


