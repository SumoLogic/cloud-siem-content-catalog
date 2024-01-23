# [Rules](README.md): LastPass - Policy Added

## Description
Detects addpolicy events from LastPass

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Defense Evasion|
|Apply Risk to Entities|user_username, srcDevice_ip|
|Signal Name|LastPass policy added by user: {{user_username}}|
|Summary Expression|LastPass policy added: {{description}}  by user: {{user_username}} from source IP: {{srcDevice_ip}}|
|Score/Severity|Static: 1|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTechnique:T1484, _mitreAttackTactic:TA0005, _mitreAttackTactic:TA0004|
## Vendors and Products


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|user_username|


