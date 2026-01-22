# [Rules](README.md): Administrative Remote Interactive Login

## Description
Detection:
This rule triggers on a successful remote interactive login (such as via RDP)  of a privileged .

Scenario:
An attacker who has obtained credentials for a privileged account proceeds to log in to one or more hosts over RDP to further their objectives.

Recommended Actions:
Note that this rule is more relevant in organizations with policies regarding acceptable use of administrative accounts. Determine whether the privileged login is normal activity by reviewing the source IP address and its geo-location, the time of day, whether the account’s role warrants login to the destination host and potentially contacting the user. If the login is not normal activity, log out all sessions for the compromised account, block the source IP address at the firewall, and review all activity by the account within the timeframe of the login.

Tuning Recommendations:
If appropriate, create a matchlist named RDP_admin_hosts and add names of hosts that are known and approved to have remote administrative logins.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Initial Access|
|Apply Risk to Entities|srcDevice_ip, user_username, dstDevice_hostname|
|Signal Name|Administrative Remote Interactive Login|
|Summary Expression|Successful administrative RDP login from IP: {{srcDevice_ip}} for user: {{user_username}}|
|Score/Severity|Static: 1|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0001, _mitreAttackTactic:TA0003, _mitreAttackTactic:TA0004, _mitreAttackTactic:TA0005, _mitreAttackTechnique:T1078, _mitreAttackTechnique:T1078.001, _mitreAttackTechnique:T1078.002, _mitreAttackTechnique:T1078.003, _mitreAttackTechnique:T1021.001, _mitreAttackTechnique:T1021, _mitreAttackTactic:TA0008|
## Vendors and Products
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|dstDevice_hostname|
|Normalized Schema|logonType|
|Normalized Schema|normalizedAction|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|success|
|Normalized Schema|user_role|
|Normalized Schema|user_username|


