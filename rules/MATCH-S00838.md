# [Rules](README.md): Azure Active Directory Authentication Method Changed

## Description
Threat actors may add rogue devices to various Azure Active Directory authentication services in order to side-step multi factor authentication controls. Added MFA devices may also serve as a persistence mechanism.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Defense Evasion|
|Apply Risk to Entities|user_username|
|Signal Name|Azure Active Directory Authentication Method Changed|
|Summary Expression|{{user_username}} has changed an authentication method in Azure Active Directory to {{description}}|
|Score/Severity|Static: 4|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0005, _mitreAttackTactic:TA0003, _mitreAttackTechnique:T1078.004|
## Vendors and Products
- [Microsoft - Azure](../products/a1225af5-e778-4068-a9a2-47da93d1ff24.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|action|
|Direct from Record|fields["properties.loggedByService"]|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|user_username|


