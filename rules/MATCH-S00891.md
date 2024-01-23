# [Rules](README.md): Azure OAUTH Application Consent from User

## Description
Depending on configurations, Azure Active Directory users or administrators may be able to consent to API permissions for various Azure AD applications, these permissions can grant adversaries access to various Azure resources, depending on the type of permissions being granted.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Defense Evasion|
|Apply Risk to Entities|user_username|
|Signal Name|Azure OAUTH Application Consent: {{application}} from {{user_username}}|
|Summary Expression|{{user_username}} has consented to application permissions|
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


