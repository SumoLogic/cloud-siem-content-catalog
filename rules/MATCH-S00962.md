# [Rules](README.md): GitHub - Repository Visibility Permissions Changed

## Description
Detects repository visibility permissions being changed to allow members of an organization to change the visibility of repositories. This activity introduces the potential for data leakage if a private or internal repository is changed to public and should be monitored to ensure no inadvertent or malicious publication of a repository. This detection was developed utilizing GitHub Enterprise Audit logging. Refer to https://help.sumologic.com/docs/integrations/app-development/github/#collecting-logs-for-github for instructions on ingesting GitHub Enterprise Audit logs.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Privilege Escalation|
|Apply Risk to Entities|user_username|
|Signal Name|GitHub - {{user_username}} Repository Visibility Change Permission Enabled for Organization Members|
|Summary Expression|{{user_username}} enabled repository visibility changes for members within the {{fields['org']}} organization.|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0004, _mitreAttackTactic:TA0010, _mitreAttackTactic:TA0005, _mitreAttackTechnique:T1562, _mitreAttackTechnique:T1222|
## Vendors and Products
- [Github - GitHub Enterprise Audit](../products/e3c8bd8b-6ed8-4332-944d-d0f5dfc462df.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|action|
|Normalized Schema|metadata_product|
|Normalized Schema|user_username|


