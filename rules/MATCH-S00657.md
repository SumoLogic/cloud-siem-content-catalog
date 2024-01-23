# [Rules](README.md): Container Running as Root

## Description
Monitors for usage of the root account within a container. This presents unnecessary risk and could also indicate a compromise where the attacker has successfully escalated privileges.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Privilege Escalation|
|Apply Risk to Entities|user_username|
|Signal Name|Container Running as Root|
|Summary Expression|Container: {{resource}} running as root|
|Score/Severity|Static: 2|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTechnique:T1078.001, _mitreAttackTechnique:T1078.004, _mitreAttackTechnique:T1078, _mitreAttackTactic:TA0004|
## Vendors and Products


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_product|
|Normalized Schema|user_username|


