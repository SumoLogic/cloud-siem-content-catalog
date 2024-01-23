# [Rules](README.md): Administrator Login via RDP

## Description
This rule looks for successful logins over RDP for administrator accounts.

## Additional Details
|Detail|Value|
|----|----|
|Type|Match|
|Category|Lateral Movement|
|Apply Risk to Entities|srcDevice_ip, user_username|
|Signal Name|Administrator Login via RDP|
|Summary Expression|Successful RDP login from IP: {{srcDevice_ip}} for user: {{user_username}}|
|Score/Severity|Static: 1|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0001, _mitreAttackTactic:TA0003, _mitreAttackTactic:TA0004, _mitreAttackTactic:TA0005, _mitreAttackTactic:TA0008, _mitreAttackTechnique:T1078, _mitreAttackTechnique:T1078.001, _mitreAttackTechnique:T1078.002, _mitreAttackTechnique:T1078.003, _mitreAttackTechnique:T1021.001, _mitreAttackTechnique:T1021|
## Vendors and Products
- [Bro - Bro](../products/37C866BF-72E1-470A-9072-EDB908F56951.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|bro_rdp_cookie|
|Normalized Schema|bro_rdp_result|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|user_username|


