# [Rules](README.md): First Seen Successful Authentication From Unexpected Country (SILENT MODE)

## Description
First Seen rule which triggers when there are at least two successful logins from the same user with different country codes indicating possible credential theft. It is recommended to add filtering criteria to the expression to reduce false positives, such as known VPN addresses.(If degradation issues occur it is recommendation implementing tuning around your expected network)

## Additional Details
|Detail|Value|
|----|----|
|Type|First Seen|
|Category|Initial Access|
|Apply Risk to Entities|user_username|
|Signal Name|First Seen Successful Authentication From Unexpected Country: {{srcDevice_ip_countryCode}} for User: {{user_username}}|
|Summary Expression|First Seen successful authentication From unexpected country for user: {{user_username}}|
|Retention Window|7776000000|
|Baseline Window|3024000000|
|Baseline Type|PER_ENTITY|
|Score/Severity|Static: 2|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0001, _mitreAttackTactic:TA0006, _mitreAttackTechnique:T1078, _mitreAttackTechnique:T1078.001, _mitreAttackTechnique:T1078.002, _mitreAttackTechnique:T1078.003, _mitreAttackTechnique:T1078.004, _mitreAttackTechnique:T1586, _mitreAttackTechnique:T1586.001, _mitreAttackTechnique:T1586.002|
## Vendors and Products
- [Druva - Druva inSync Cloud](../products/2d47fe59-4607-48f7-a21a-eb3f5f051660.md)
- [Microsoft - Azure](../products/a1225af5-e778-4068-a9a2-47da93d1ff24.md)
- [Okta - Single Sign-On](../products/51278354-d6b5-4c8e-a8fd-8197df334e67.md)
- [Palo Alto Networks - GlobalProtect](../products/b0fe0dde-4e19-4712-957b-1ea7418c132e.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|normalizedAction|
|Normalized Schema|objectType|
|Normalized Schema|srcDevice_ip_countryCode|
|Normalized Schema|srcDevice_ip_isInternal|
|Normalized Schema|success|
|Normalized Schema|user_username|


