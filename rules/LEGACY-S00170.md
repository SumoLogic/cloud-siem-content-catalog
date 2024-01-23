# [Rules](README.md): The Audit Log was Cleared - 1102

## Description
Attackers may attempt to clear the Windows Security Event Log in an effort to hide records of their activity during an intrusion. This rule detects that action.

## Additional Details
|Detail|Value|
|----|----|
|Type|Match|
|Category|Defense Evasion|
|Apply Risk to Entities|device_hostname, device_ip, user_username|
|Signal Name|The Audit Log was Cleared - 1102|
|Summary Expression|Windows Event Log cleared on host: {{device_hostname}}|
|Score/Severity|Static: 10|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0005, _mitreAttackTechnique:T1070, _mitreAttackTechnique:T1070.001, _mitreAttackTechnique:T1070.003|
## Vendors and Products
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Direct from Record|fields['Provider.Name']|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|user_username|


