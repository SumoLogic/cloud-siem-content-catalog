# [Rules](README.md): LastPass - Master Password Changed

## Description
Detects masterpasswordchanged events from LastPass

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Persistence|
|Apply Risk to Entities|user_username, srcDevice_ip|
|Signal Name|LastPass master password changed for user: {{user_username}}|
|Summary Expression|LastPass master password changed for user: {{user_username}} from source IP: {{srcDevice_ip}}|
|Score/Severity|Static: 2|
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


