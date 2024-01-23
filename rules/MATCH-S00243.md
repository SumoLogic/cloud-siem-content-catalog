# [Rules](README.md): Azure - High Risk Sign-In (Aggregate)

## Description
Detects Azure high aggregate risk for a user sign in. https://docs.microsoft.com/en-us/azure/active-directory/identity-protection/troubleshooting-identity-protection-faq

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Initial Access|
|Apply Risk to Entities|device_hostname, device_ip, user_username, srcDevice_ip|
|Signal Name|Azure - High Risk Sign-In (Aggregate)|
|Summary Expression|A sign-in from user: {{user_username}} on IP: {{device_ip}} with a high aggregate risk level was detected.|
|Score/Severity|Static: 3|
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
|Direct from Record|fields['properties.riskLevelAggregated']|
|Direct from Record|fields['riskLevelAggregated']|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|objectType|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|success|
|Normalized Schema|user_username|


