# [Rules](README.md): First Seen whoami command From User

## Description
Observes for a user performing a whoami command for the first time.

## Additional Details
|Detail|Value|
|----|----|
|Type|First Seen|
|Category|Discovery|
|Apply Risk to Entities|user_username|
|Signal Name|First Seen whoami command From User|
|Summary Expression|First Seen use of whoami executed by the user: {{user_username}}|
|Retention Window|7776000000|
|Baseline Window|1209600000|
|Baseline Type|GLOBAL|
|Score/Severity|Static: 1|
|Enabled by Default|True|
|Prototype|True|
|Tags|_mitreAttackTactic:TA0007, _mitreAttackTechnique:T1033|
## Vendors and Products
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|user_username|


