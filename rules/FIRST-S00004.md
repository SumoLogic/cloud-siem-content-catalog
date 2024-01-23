# [Rules](README.md): First Seen Local Group Addition by User

## Description
Observes for a user being added to a security-enabled local group in Windows

## Additional Details
|Detail|Value|
|----|----|
|Type|First Seen|
|Category|Privilege Escalation|
|Apply Risk to Entities|user_username|
|Signal Name|First Seen Local Group Addition by User|
|Summary Expression|First Seen addition to a local Windows group: {{targetUser_username}} for user: {{user_username}}|
|Retention Window|7776000000|
|Baseline Window|3024000000|
|Baseline Type|GLOBAL|
|Score/Severity|Static: 2|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0004, _mitreAttackTactic:TA0003, _mitreAttackTechnique:T1078, _mitreAttackTechnique:T1078.003|
## Vendors and Products
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|user_username|


