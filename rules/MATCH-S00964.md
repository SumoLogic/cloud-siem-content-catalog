# [Rules](README.md): GitHub - SSO Recovery Codes Access Activity

## Description
Detects activities accessing SSO recovery codes. SSO recovery codes can enable a user to bypass normal more stringent authentication routes. This detection was developed utilizing GitHub Enterprise Audit logging. Refer to https://help.sumologic.com/docs/integrations/app-development/github/#collecting-logs-for-github for instructions on ingesting GitHub Enterprise Audit logs.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Initial Access|
|Apply Risk to Entities|user_username|
|Signal Name|GitHub - {{user_username}}  Performed a {{action}} Activity|
|Summary Expression|{{action}} performed by {{user_username}} on the {{fields['org']}} organization|
|Score/Severity|Static: 4|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0001, _mitreAttackTactic:TA0006, _mitreAttackTactic:TA0005, _mitreAttackTechnique:T1548.002, _mitreAttackTechnique:T1548|
## Vendors and Products
- [Github - GitHub Enterprise Audit](../products/e3c8bd8b-6ed8-4332-944d-d0f5dfc462df.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|action|
|Normalized Schema|metadata_product|
|Normalized Schema|user_username|


