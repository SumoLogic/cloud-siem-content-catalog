# [Rules](README.md): GitHub - Administrator Added or Invited

## Description
Detects additions or invitations of GitHub Administrators. Illegitimate addition of administrative users could be an indication of priviledge escalation or persistence by adversaries.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Persistence|
|Apply Risk to Entities|user_username, targetUser_username|
|Signal Name|GitHub - {{targetUser_username}} Added or Invited as a GitHub Administrator|
|Summary Expression|{{user_username}} added or invited {{targetUser_username}} as a GitHub administrator for {{fields['business']}}|
|Score/Severity|Static: 2|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0003, _mitreAttackTactic:TA0004, _mitreAttackTechnique:T1078|
## Vendors and Products
- [Github - GitHub Enterprise Audit](../products/e3c8bd8b-6ed8-4332-944d-d0f5dfc462df.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|action|
|Normalized Schema|metadata_product|
|Normalized Schema|targetUser_username|
|Normalized Schema|user_username|


