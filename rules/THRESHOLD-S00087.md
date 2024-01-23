# [Rules](README.md): Slack - Possible Session Hijacking

## Description
Detects the same sessionID used from a new IP for the same user in a short period of time.

## Additional Details
|Detail|Value|
|----|----|
|Type|Threshold|
|Category|Credential Access|
|Apply Risk to Entities|user_username|
|Signal Name|Slack - Possible Session Hijacking|
|Summary Expression|User: {{user_username}} potential session hijack|
|Threshold Count|2|
|Threshold Window|60m|
|Score/Severity|Static: 5|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0006, _mitreAttackTechnique:T1539|
## Vendors and Products


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|device_ip|
|Normalized Schema|device_ip_asnNumber|
|Normalized Schema|device_ip_asnOrg|
|Normalized Schema|metadata_vendor|
|Normalized Schema|user_username|


