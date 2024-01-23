# [Rules](README.md): Azure PRT Token Issued via Non Interactive Login

## Description
Azure Primary Refresh Tokens (PRT) can be used to authenticate  to Azure Active Directory and Azure compute resources. This rule looks for a PRT token successfully issued via a non-interactive login and when a suspicious User Agent is in use.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Initial Access|
|Apply Risk to Entities|srcDevice_ip, user_username|
|Signal Name|Azure PRT Token Issued via Non Interactive Login|
|Summary Expression|A suspicious Azure Primary Refersh Token (PRT) was issued via non-interactive login to {{user_username}} for the {{application}} resource.|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0001, _mitreAttackTechnique:T1078, ta, _mitreAttackTactic:TA0007, _mitreAttackTechnique:T1526, _mitreAttackTechnique:T1098|
## Vendors and Products
- [Microsoft - Azure](../products/a1225af5-e778-4068-a9a2-47da93d1ff24.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|application|
|Normalized Schema|errorCode|
|Direct from Record|fields['properties.incomingTokenType']|
|Direct from Record|fields['properties.userAgent']|
|Normalized Schema|logonType|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|user_username|


