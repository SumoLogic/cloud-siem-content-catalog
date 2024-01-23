# [Rules](README.md): Rubeus Hack Tool Logon Process Name

## Description
From FireEye Red Team Tool Countermeasures:
Rubeus is a utility  that provides Kerberos abuse capabilities. This rule is looking for the  hardcoded LogonProcessName value, "User32LogonProcesss".

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Privilege Escalation|
|Apply Risk to Entities|device_ip, device_hostname, srcDevice_hostname, srcDevice_ip, user_username|
|Signal Name|Rubeus Hack Tool Logon Process Name|
|Summary Expression|Rubeus hack tool indicator detected on host: {{device_hostname}}|
|Score/Severity|Static: 5|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0004, _mitreAttackTactic:TA0005, _mitreAttackTactic:TA0006, _mitreAttackTactic:TA0008, _mitreAttackTechnique:T1550, _mitreAttackTechnique:T1550.003, _mitreAttackTechnique:T1558, _mitreAttackTechnique:T1558.003|
## Vendors and Products
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Direct from Record|fields['EventData.LogonProcessName']|
|Normalized Schema|objectType|
|Normalized Schema|srcDevice_hostname|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|user_username|


