# [Rules](README.md): GitHub - Repository Visibility Changed to Public

## Description
Detects a user making a repository public. This action should be closely monitored and mitigative actions taken even if the published repository is deleted, or reverted to private. Reference: https://trufflesecurity.com/blog/anyone-can-access-deleted-and-private-repo-data-github. This detection was developed utilizing GitHub Enterprise Audit logging. Refer to https://help.sumologic.com/docs/integrations/app-development/github/#collecting-logs-for-github for instructions on ingesting GitHub Enterprise Audit logs.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Exfiltration|
|Apply Risk to Entities|user_username, repository|
|Signal Name|GitHub - {{repository}} Visibility Changed to Public|
|Summary Expression|Repository: {{repository}} made public by {{user_username}}|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0010, _mitreAttackTechnique:T1213|
## Vendors and Products
- [Github - GitHub Enterprise Audit](../products/e3c8bd8b-6ed8-4332-944d-d0f5dfc462df.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|action|
|Direct from Record|fields['visibility']|
|Normalized Schema|metadata_product|
|Normalized Schema|repository|
|Normalized Schema|user_username|


