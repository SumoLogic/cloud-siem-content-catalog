# [Rules](README.md): GitHub - Member Permissions Modification

## Description
Detects modifications of GitHub user permissions. Added permissions for a user should be monitored for potential privilege escalation by an adversary. This detection was developed utilizing GitHub Enterprise Audit logging. Refer to https://help.sumologic.com/docs/integrations/app-development/github/#collecting-logs-for-github for instructions on ingesting GitHub Enterprise Audit logs.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Privilege Escalation|
|Apply Risk to Entities|user_username, targetUser_username, srcDevice_ip|
|Signal Name|GitHub - {{targetUser_username}}  Permissions Modified|
|Summary Expression|{{user_username}}  modified the GitHub permissions of {{targetUser_username}} from {{fields['old_permission']}}  to {{targetUser_role}}  on the {{fields['org']}} organization|
|Score/Severity|Dynamic: 0 or 1 or 2 or 3 or 4 or 5|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0004, _mitreAttackTechnique:T1098|
## Vendors and Products
- [Github - GitHub Enterprise Audit](../products/e3c8bd8b-6ed8-4332-944d-d0f5dfc462df.md)


## Dynamic Signal Score/Severity Translation

The default score of `0` is used as a catch all if none of the translations are met.

|Schema Field|Field Value|Score/Severity|
|------------|-----------|--------------|
|targetUser_role|admin|5|
|targetUser_role|maintainer|4|
|targetUser_role|push|3|
|targetUser_role|triage|2|
|targetUser_role|pull|1|
## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|action|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|targetUser_role|
|Normalized Schema|targetUser_username|
|Normalized Schema|user_username|


