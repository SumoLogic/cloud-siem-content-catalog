# [Rules](README.md): Azure - Risky User State : User Confirmed Compromised

## Description
This rule detects that an administrator has flagged a sign-in in Identity Protection as not having been performed by the account owner, indicating a compromise.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Initial Access|
|Apply Risk to Entities|device_hostname, device_ip, user_username, srcDevice_ip|
|Signal Name|Azure - User Confirmed Compromised|
|Summary Expression|Administrator flagged sign in by {{user_username}} was not performed by the account owner|
|Score/Severity|Static: 5|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0001, _mitreAttackTactic:TA0003, _mitreAttackTactic:TA0004, _mitreAttackTactic:TA0005, _mitreAttackTactic:TA0042, _mitreAttackTechnique:T1078, _mitreAttackTechnique:T1586, _mitreAttackTechnique:T1586.002, _mitreAttackTechnique:T1078.002, _mitreAttackTechnique:T1078.004|
## Vendors and Products
- [Microsoft - Azure](../products/a1225af5-e778-4068-a9a2-47da93d1ff24.md)
- [Microsoft - Graph AD Reporting API](../products/fe5a3e8b-8b6e-44c7-92a8-adfb20df5c75.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Direct from Record|fields['properties.riskDetail']|
|Direct from Record|fields['riskDetail']|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|objectType|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|user_username|


