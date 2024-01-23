# [Rules](README.md): Potential Azure Persistence via Automation Accounts

## Description
Azure automation accounts are normally used for automation of various tasks, however, they can also be abused to create Azure Active Directory accounts for threat actor persistence.

## Additional Details
|Detail|Value|
|----|----|
|Type|Chain|
|Category|Persistence|
|Apply Risk to Entities|user_username|
|Signal Name|Potential Azure Persistence via Automation Accounts|
|Summary Expression|Potential Azure Persistence via Automation Accounts|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0003, _mitreAttackTechnique:T1078, _mitreAttackTactic:TA0005, _mitreAttackTechnique:T1078.004|
## Vendors and Products
- [Microsoft - Azure](../products/a1225af5-e778-4068-a9a2-47da93d1ff24.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|description|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|success|
|Normalized Schema|user_username|


