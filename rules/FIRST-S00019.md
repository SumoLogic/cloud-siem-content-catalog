# [Rules](README.md): First Seen Azure Member Addition to Group from User

## Description
Detects a user being added to a group for the first time by a user. This may be a routine activity, but could be indicative of an attempt to escalate account privileges. It is recommended to add additional expression logic to this rule to either exclude non-sensitive groups, or to only include sensitive groups.

## Additional Details
|Detail|Value|
|----|----|
|Type|First Seen|
|Category|Privilege Escalation|
|Apply Risk to Entities|user_username|
|Signal Name|First Seen Azure Member Addition to Group from User|
|Summary Expression|{{user_username}} added {{changeTarget}} to group|
|Retention Window|7776000000|
|Baseline Window|1209600000|
|Baseline Type|GLOBAL|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0004, _mitreAttackTechnique:T1078, _mitreAttackTechnique:T1078.004, _mitreAttackTechnique:T1098, _mitreAttackTechnique:T1098.003|
## Vendors and Products
- [Microsoft - Azure](../products/a1225af5-e778-4068-a9a2-47da93d1ff24.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|changeType|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|user_username|


