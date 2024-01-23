# [Rules](README.md): Attempt to Clear Windows Event Logs Using Wevtutil

## Description
Observes for attempts to clear Windows event logs using wevtutil.

Command line auditing is necessary for this rule to function.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Defense Evasion|
|Apply Risk to Entities|device_hostname, device_ip, user_username|
|Signal Name|Attempt to Clear Windows Event Logs Using Wevtutil|
|Summary Expression|Attempt to clear Windows Event Log on host: {{device_hostname}} by user: {{user_username}}|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0005, _mitreAttackTechnique:T1070, _mitreAttackTechnique:T1070.001|
## Vendors and Products
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|baseImage|
|Normalized Schema|commandLine|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|user_username|


