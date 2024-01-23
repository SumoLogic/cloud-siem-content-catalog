# [Rules](README.md): AWS CloudTrail - Reconnaissance related event

## Description
This signal identifies a small number of CloudTrail API actions that when observed could indicate an actors intent to enumerate the environment.  These events are generally benign, and occur during normal operations.  Use this signal as context around an unfolding security story.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Discovery|
|Apply Risk to Entities|device_hostname, device_ip, user_username, srcDevice_ip|
|Signal Name|AWS CloudTrail - Reconnaissance related event|
|Summary Expression|{{action}} performed by user: {{user_username}}|
|Score/Severity|Static: 1|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0007, _mitreAttackTechnique:T1069, _mitreAttackTechnique:T1087, _mitreAttackTechnique:T1526, _mitreAttackTechnique:T1087.004, _mitreAttackTechnique:T1069.003|
## Vendors and Products
- [Amazon AWS - CloudTrail](../products/033624b0-218e-4dcb-b93f-0f1fb1806c56.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|listMatches|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|user_username|


