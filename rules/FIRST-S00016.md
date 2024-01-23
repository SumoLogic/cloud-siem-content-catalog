# [Rules](README.md): First Seen Non-Network/Non-System Logon from User

## Description
First Seen Non-Network Logon from User

## Additional Details
|Detail|Value|
|----|----|
|Type|First Seen|
|Category|Credential Access|
|Apply Risk to Entities|user_username|
|Signal Name|First Seen Non-Network/Non-System Logon from User|
|Summary Expression|First Seen Non-Network Logon by user {{user_username}}|
|Retention Window|7776000000|
|Baseline Window|1209600000|
|Baseline Type|PER_ENTITY|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0006|
## Vendors and Products
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|logonType|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|user_username|


