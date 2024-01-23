# [Rules](README.md): First Seen User Creation From User

## Description
Observes for a user being created for the first time by a user previously unassociated with account creation

## Additional Details
|Detail|Value|
|----|----|
|Type|First Seen|
|Category|Persistence|
|Apply Risk to Entities|user_username|
|Signal Name|First Seen User Creation From User|
|Summary Expression|First Seen creation of a user: {{targetUser_username}} by the user: {{user_username}}|
|Retention Window|7776000000|
|Baseline Window|1209600000|
|Baseline Type|GLOBAL|
|Score/Severity|Static: 4|
|Enabled by Default|True|
|Prototype|True|
|Tags|_mitreAttackTactic:TA0003|
## Vendors and Products
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|user_username|


