# [Rules](README.md): GitHub - Secret Scanning Alert

## Description
Observes for secret scanning alerts from GitHub. Secrets detected by GitHub Enterprise Cloud undergo validation by GitHub automatically, to determine whether they are actively in use, this is not surfaced in the audit log, and will require separate inspection. For more information see : [Evaluating alerts from secret scanning](https://docs.github.com/en/code-security/secret-scanning/managing-alerts-from-secret-scanning/evaluating-alerts). This detection was developed utilizing GitHub Enterprise Audit logging. Refer to https://help.sumologic.com/docs/integrations/app-development/github/#collecting-logs-for-github for instructions on ingesting GitHub Enterprise Audit logs.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Credential Access|
|Apply Risk to Entities|repository|
|Signal Name|GitHub - Detected a {{fields['secret_type_display_name']}} secret on {{repository}}|
|Summary Expression|GitHub has generated secret scanning alert #{{fields['number']}} for the {{fields['repository']}} within the {{fields['org']}} organization|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0006, _mitreAttackTechnique:T1552.004, _mitreAttackTechnique:T1552|
## Vendors and Products
- [Github - GitHub Enterprise Audit](../products/e3c8bd8b-6ed8-4332-944d-d0f5dfc462df.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|action|
|Direct from Record|fields['secret_type_display_name']|
|Normalized Schema|metadata_product|
|Normalized Schema|repository|


