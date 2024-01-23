# [Rules](README.md): Salesforce Login Attempt from Disabled Account

## Description
Detects when a disabled account attempts to log into Salesforce

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Initial Access|
|Apply Risk to Entities|srcDevice_ip, user_username|
|Signal Name|Salesforce Login Attempt from Disabled Account|
|Summary Expression|Salesforce Login Attempt from Disabled Account: {{user_username}} IP: {{srcDevice_ip}}|
|Score/Severity|Static: 4|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0001, _mitreAttackTechnique:T1078.004, _mitreAttackTactic:TA0006, _mitreAttackTechnique:T1078|
## Vendors and Products


## Fields Used

|Origin|Field|
|----|----|
|Direct from Record|fields['LOGIN_STATUS']|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|user_username|


