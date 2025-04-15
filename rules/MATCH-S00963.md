# [Rules](README.md): GitHub - SSH Key Created for Private Repo

## Description
Detects the creation of an SSH key for a private GitHub repository.  Performed maliciously, creating an SSH key could create a parallel access path for an attacker. This detection was developed utilizing GitHub Enterprise Audit logging. Refer to https://help.sumologic.com/docs/integrations/app-development/github/#collecting-logs-for-github for instructions on ingesting GitHub Enterprise Audit logs.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Persistence|
|Apply Risk to Entities|user_username|
|Signal Name|GitHub - SSH Key Created for Private Repo by {{user_username}}|
|Summary Expression|{{user_username}}  created {{fields['title']}} for the {{repository}} private repository|
|Score/Severity|Static: 2|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0003, _mitreAttackTactic:TA0006, _mitreAttackTechnique:T1098, _mitreAttackTechnique:T1098.004|
## Vendors and Products
- [Github - GitHub Enterprise Audit](../products/e3c8bd8b-6ed8-4332-944d-d0f5dfc462df.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|action|
|Direct from Record|fields['public_repo']|
|Normalized Schema|metadata_product|
|Normalized Schema|user_username|


