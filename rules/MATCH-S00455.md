# [Rules](README.md): O365 - Successful Authentication with PowerShell User Agent

## Description
Detects a successful authentication to Office 365 where the user agent string contains PowerShell. By default, PowerShell will appear in the user agent string when used in authentication attempts for 0365. This can be an indication of a PowerShell Exploitation framework being used to authenticate.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Credential Access|
|Apply Risk to Entities|device_ip, user_username|
|Signal Name|O365 - Successful Authentication with PowerShell User Agent|
|Summary Expression|User: {{user_username}} successfully logged on|
|Score/Severity|Static: 5|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0001, _mitreAttackTactic:TA0003, _mitreAttackTactic:TA0004, _mitreAttackTactic:TA0005, _mitreAttackTactic:TA0006, _mitreAttackTechnique:T1078, _mitreAttackTechnique:T1078.004|
## Vendors and Products
- [Microsoft - Office 365](../products/d3ed003d-5ddd-4c7a-bea5-63eae6311833.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|device_ip|
|Direct from Record|fields['ExtendedProperties.1.Value']|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|success|
|Normalized Schema|user_username|


