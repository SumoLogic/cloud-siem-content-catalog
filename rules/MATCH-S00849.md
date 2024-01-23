# [Rules](README.md): LastPass - Personal Share

## Description
Detects personalshare events from LastPass

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Persistence|
|Apply Risk to Entities|user_username, srcDevice_ip|
|Signal Name|LastPass personal share by user: {{user_username}}|
|Summary Expression|LastPass personal share by user: {{user_username}} to user: {{description}}|
|Score/Severity|Static: 1|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0003, _mitreAttackTechnique:T1098|
## Vendors and Products


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|user_username|


