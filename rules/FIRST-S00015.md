# [Rules](README.md): First Seen Macro Execution from User

## Description
First Seen Macro Execution from User

## Additional Details
|Detail|Value|
|----|----|
|Type|First Seen|
|Category|Execution|
|Apply Risk to Entities|user_username|
|Signal Name|First Seen Macro Execution from User|
|Summary Expression|First Seen Macro Execution by user {{user_username}}|
|Retention Window|7776000000|
|Baseline Window|1209600000|
|Baseline Type|GLOBAL|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0002|
## Vendors and Products
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|action|
|Normalized Schema|user_username|


