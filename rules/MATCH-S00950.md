# [Rules](README.md): GitHub - Member Invitation or Addition

## Description
Detects new user additions or invitations to the business or organizations GitHub. New user additions/invitations should be monitored as they could be a vector for malicious actors to establish access or persistence. This detection was developed utilizing GitHub Enterprise Audit logging. Refer to https://help.sumologic.com/docs/integrations/app-development/github/#collecting-logs-for-github for instructions on ingesting GitHub Enterprise Audit logs.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Initial Access|
|Apply Risk to Entities|user_username, targetUser_username|
|Signal Name|GitHub - User {{targetUser_username}} was Added or Invited to the {{fields['org']}}|
|Summary Expression|{{user_username}}  invited or added {{targetUser_username}}  to the {{fields['org']}}  organization within the {{fields['business']}}  business|
|Score/Severity|Static: 0|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0001, _mitreAttackTactic:TA0003, _mitreAttackTechnique:T1098|
## Vendors and Products
- [Github - GitHub Enterprise Audit](../products/e3c8bd8b-6ed8-4332-944d-d0f5dfc462df.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|action|
|Direct from Record|fields['org']|
|Normalized Schema|metadata_product|
|Normalized Schema|targetUser_username|
|Normalized Schema|user_username|


