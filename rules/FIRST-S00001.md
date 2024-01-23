# [Rules](README.md): First Seen Administrative Privileges Granted for User

## Description
Observes for granting of administrative privileges in Windows for the first time for a given user

## Additional Details
|Detail|Value|
|----|----|
|Type|First Seen|
|Category|Privilege Escalation|
|Apply Risk to Entities|user_username|
|Signal Name|First Seen Administrative Privileges Granted for User|
|Summary Expression|First Seen administrative privileges granted for user: {{user_username}}|
|Retention Window|7776000000|
|Baseline Window|2592000000|
|Baseline Type|GLOBAL|
|Score/Severity|Static: 2|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0004|
## Vendors and Products
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|user_username|


