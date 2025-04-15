# [Rules](README.md): GitHub - Secret Scanning Potentially Disabled

## Description
Detects actions which disable or modify secret scanning policies for an organization or repository. Modifying or disabling secret scanning may lead to inadvertent leaking of credentials. This detection was developed utilizing GitHub Enterprise Audit logging. Refer to https://help.sumologic.com/docs/integrations/app-development/github/#collecting-logs-for-github for instructions on ingesting GitHub Enterprise Audit logs.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Defense Evasion|
|Apply Risk to Entities|user_username, repository|
|Signal Name|GitHub - {{user_username}} performed a {{action}}|
|Summary Expression|{{user_username}} performed a {{action}}  within the {{fields['org']}} organization|
|Score/Severity|Dynamic: 3 or 4|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0005, _mitreAttackTechnique:T1552.004, _mitreAttackTechnique:T1552|
## Vendors and Products
- [Github - GitHub Enterprise Audit](../products/e3c8bd8b-6ed8-4332-944d-d0f5dfc462df.md)


## Dynamic Signal Score/Severity Translation

The default score of `3` is used as a catch all if none of the translations are met.

|Schema Field|Field Value|Score/Severity|
|------------|-----------|--------------|
|action|org_secret_scanning_generic_secrets.disabled|4|
|action|org.secret_scanning_push_protection_disable|4|
## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|action|
|Normalized Schema|metadata_product|
|Normalized Schema|repository|
|Normalized Schema|user_username|


