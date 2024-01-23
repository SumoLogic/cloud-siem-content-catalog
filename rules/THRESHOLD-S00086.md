# [Rules](README.md): Slack - Mass Download Events

## Description
Adversaries may use an existing, legitimate external Web service to exfiltrate data rather than their primary command and control channel.

## Additional Details
|Detail|Value|
|----|----|
|Type|Threshold|
|Category|Exfiltration|
|Apply Risk to Entities|user_username|
|Signal Name|Slack - Mass Download Events|
|Summary Expression|User: {{user_username}} downloaded multiple files|
|Threshold Count|10|
|Threshold Window|30m|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTechnique:T1567, _mitreAttackTechnique:T1048, _mitreAttackTechnique:T1048.003, _mitreAttackTechnique:T1567.002, _mitreAttackTactic:TA0010|
## Vendors and Products


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|action|
|Normalized Schema|metadata_vendor|
|Normalized Schema|user_username|


