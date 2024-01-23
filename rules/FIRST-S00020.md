# [Rules](README.md): First Seen Azure OAUTH Application Consent from User

## Description
A user has consented to application permissions for the first time since the baseline period occurred.

## Additional Details
|Detail|Value|
|----|----|
|Type|First Seen|
|Category|Defense Evasion|
|Apply Risk to Entities|user_username|
|Signal Name|First Seen Azure OAUTH Application Consent: {{application}} from User|
|Summary Expression|Depending on configurations, Azure Active Directory users or administrators may be able to consent to API permissions for various Azure AD applications, these permissions can grant adversaries access to various Azure resources, depending on the type of permissions being granted.|
|Retention Window|7776000000|
|Baseline Window|1209600000|
|Baseline Type|PER_ENTITY|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0005, _mitreAttackTactic:TA0008, _mitreAttackTechnique:T1550.001|
## Vendors and Products
- [Microsoft - Azure](../products/a1225af5-e778-4068-a9a2-47da93d1ff24.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|action|
|Normalized Schema|application|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|objectType|
|Normalized Schema|user_username|


