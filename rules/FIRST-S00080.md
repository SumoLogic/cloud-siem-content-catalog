# [Rules](README.md): First Seen Azure Portal access by User

## Description
First observance of a user logging on to the Microsoft Azure Portal. This could be indicative of new user onboarding, or an unauthorized access to the Azure portal. Recommended to investigate the nature of the user account and the login.

## Additional Details
|Detail|Value|
|----|----|
|Type|First Seen|
|Category|Discovery|
|Apply Risk to Entities|user_username|
|Signal Name|First Seen Azure Portal by User: {{user_username}}|
|Summary Expression|First Seen Azure Portal access by {{user_username}}|
|Retention Window|7776000000|
|Baseline Window|2592000000|
|Baseline Type|GLOBAL|
|Score/Severity|Static: 1|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0007, _mitreAttackTechnique:T1538|
## Vendors and Products
- [Microsoft - Azure](../products/a1225af5-e778-4068-a9a2-47da93d1ff24.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|application|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|objectType|
|Normalized Schema|success|
|Normalized Schema|user_username|


