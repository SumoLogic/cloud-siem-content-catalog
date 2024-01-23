# [Rules](README.md): LastPass - Failed Login

## Description
Detects Failed Login events from LastPass

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Credential Access|
|Apply Risk to Entities|user_username, srcDevice_ip|
|Signal Name|LastPass Failed Login by user: {{user_username}}|
|Summary Expression|LastPass Failed Login: {{description}}  by user: {{user_username}} from source IP: {{srcDevice_ip}}|
|Score/Severity|Static: 1|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0006|
## Vendors and Products


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|user_username|


