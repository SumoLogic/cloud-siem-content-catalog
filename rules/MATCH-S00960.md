# [Rules](README.md): GitHub - Repository Transfer

## Description
Detects transfers of a repository to another organization or user. This is a sensitive activity that GitHub places in the "Danger Zone" of repository setting and should be monitored to ensure no unauthorized transfers are taking place. This detection was developed utilizing GitHub Enterprise Audit logging. Refer to https://help.sumologic.com/docs/integrations/app-development/github/#collecting-logs-for-github for instructions on ingesting GitHub Enterprise Audit logs.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Lateral Movement|
|Apply Risk to Entities|user_username|
|Signal Name|GitHub - {{user_username}} Transferred a Repository to another Organization or User|
|Summary Expression|{{user_username}} transferred the {{repository}} from{{fields['repo_was']}} to {{fields['new_nwo']}}|
|Score/Severity|Static: 4|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0008, _mitreAttackTechnique:T1537, _mitreAttackTactic:TA0010|
## Vendors and Products
- [Github - GitHub Enterprise Audit](../products/e3c8bd8b-6ed8-4332-944d-d0f5dfc462df.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|action|
|Normalized Schema|metadata_product|
|Normalized Schema|user_username|


