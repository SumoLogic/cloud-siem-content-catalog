# [Rules](README.md): GitHub - Two-Factor Authentication Disabled for Organization

## Description
Observes for two-factor authentication being disabled for a GitHub organization. Removing two-factor authentication requirements significantly degrades the security of the GitHub organization by permitting password only authentication. This detection was developed utilizing GitHub Enterprise Audit logging. Refer to https://help.sumologic.com/docs/integrations/app-development/github/#collecting-logs-for-github for instructions on ingesting GitHub Enterprise Audit logs.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Credential Access|
|Apply Risk to Entities|user_username|
|Signal Name|GitHub -{{user_username}} disabled Two-Factor Authentication for the {{fields['org']}} organization|
|Summary Expression|User:{{user_username}} has disabled Two-Factor Authentication for the {{fields['org']}} organization from {{srcDevice_ip}}|
|Score/Severity|Static: 6|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0006, _mitreAttackTechnique:T1556, _mitreAttackTechnique:T1556.006|
## Vendors and Products
- [Github - GitHub Enterprise Audit](../products/e3c8bd8b-6ed8-4332-944d-d0f5dfc462df.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|action|
|Direct from Record|fields['org']|
|Normalized Schema|metadata_product|
|Normalized Schema|user_username|


