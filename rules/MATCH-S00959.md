# [Rules](README.md): GitHub - Repository Public Key Deletion

## Description
Detects deletions of SSH keys in GitHub. Unusual deletions could represent an adversary attempting to disrupt normal operations by denying access. This detection was developed utilizing GitHub Enterprise Audit logging. Refer to https://help.sumologic.com/docs/integrations/app-development/github/#collecting-logs-for-github for instructions on ingesting GitHub Enterprise Audit logs.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Impact|
|Apply Risk to Entities|user_username, repository|
|Signal Name|GitHub - {{user_username}} Deleted a Repository Key|
|Summary Expression|{{user_username}} Deleted Repository Key {{fields['title']}} . Explanation: {{fields['explanation']}}|
|Score/Severity|Static: 4|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0040, _mitreAttackTechnique:T1485|
## Vendors and Products
- [Github - GitHub Enterprise Audit](../products/e3c8bd8b-6ed8-4332-944d-d0f5dfc462df.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|action|
|Direct from Record|fields['explanation']|
|Normalized Schema|metadata_product|
|Normalized Schema|repository|
|Normalized Schema|user_username|


