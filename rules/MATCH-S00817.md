# [Rules](README.md): Suspicious Azure Active Directory Device Code Authentication

## Description
Successful Device Code authentication flows result in the issuance of an Azure Primary Refresh Token which can be used to access, enumerate or - if the relevant permissions exist - to modify Azure resources.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Initial Access|
|Apply Risk to Entities|srcDevice_ip, user_username|
|Signal Name|Suspicious Azure Active Directory Device Code Authentication|
|Summary Expression|A successful & suspcious Device Code authentication flow was completed to access the Azure resource: {{application}} for the user: {{user_username}}|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0001, _mitreAttackTactic:TA0007, _mitreAttackTechnique:T1526, _mitreAttackTechnique:T1098|
## Vendors and Products
- [Microsoft - Azure](../products/a1225af5-e778-4068-a9a2-47da93d1ff24.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|errorCode|
|Direct from Record|fields['properties.appDisplayName']|
|Direct from Record|fields['properties.authenticationProtocol']|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|user_username|


