# [Rules](README.md): AWS CloudTrail - Aggressive Reconnaissance

## Description
This signal identifies when a large variety of different AWS CloudTrail event ids are observed in a short period of time.  The event id's are generally related to reconnaissance.  This signal can indicate that an aggressive scan of AWS resources is underway.

## Additional Details
|Detail|Value|
|----|----|
|Type|Aggregation|
|Category|Discovery|
|Apply Risk to Entities|device_hostname, device_ip, user_username, srcDevice_ip|
|Signal Name|AWS CloudTrail - Aggressive Reconnaissance|
|Summary Expression|AWS CloudTrail reconnaissance activity detected by user: {{user_username}} from source IP: {{srcDevice_ip}}|
|Aggregation Window|30m|
|Score/Severity|Static: 1|
|Enabled by Default|True|
|Prototype|True|
|Tags|_mitreAttackTactic:TA0007, _mitreAttackTechnique:T1069, _mitreAttackTechnique:T1087, _mitreAttackTechnique:T1069.003, _mitreAttackTechnique:T1087.004|
## Vendors and Products
- [Amazon AWS - CloudTrail](../products/033624b0-218e-4dcb-b93f-0f1fb1806c56.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|distinct_eventid_count|
|Normalized Schema|listMatches|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|user_username|


