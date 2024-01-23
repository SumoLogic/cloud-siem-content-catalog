# [Rules](README.md): Change of Azure MFA Method followed by Risky SignIn

## Description
This alert looks for an Azure MFA authentication method change, followed by a risky sign in detected by Azure within a six hour time period for the same user account.

## Additional Details
|Detail|Value|
|----|----|
|Type|Chain|
|Category|Persistence|
|Apply Risk to Entities|user_username|
|Signal Name|Change of Azure MFA Method followed by Risky SignIn|
|Summary Expression|Change of Azure MFA Method followed by Risky Sign-In by {{user_username}}|
|Score/Severity|Static: 7|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0003, _mitreAttackTechnique:T1078.004|
## Vendors and Products
- [Microsoft - Azure](../products/a1225af5-e778-4068-a9a2-47da93d1ff24.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|action|
|Direct from Record|fields["properties.loggedByService"]|
|Normalized Schema|logonType|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|user_username|


