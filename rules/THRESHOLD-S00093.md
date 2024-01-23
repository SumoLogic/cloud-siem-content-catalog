# [Rules](README.md): AWS Route 53 Reconnaissance

## Description
Detects a variety of AWS Route 53 API actions that when observed together could indicate an actors intent to enumerate the environment.

## Additional Details
|Detail|Value|
|----|----|
|Type|Threshold|
|Category|Discovery|
|Apply Risk to Entities|device_hostname, device_ip, srcDevice_ip, srcDevice_hostname, user_username|
|Signal Name|AWS Route 53 Reconnaissance|
|Summary Expression|AWS Route 53 actions performed by user: {{user_username}}|
|Threshold Count|3|
|Threshold Window|60m|
|Score/Severity|Static: 4|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0007, _mitreAttackTechnique:T1526|
## Vendors and Products
- [Amazon AWS - CloudTrail](../products/033624b0-218e-4dcb-b93f-0f1fb1806c56.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|action|
|Normalized Schema|application|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|listMatches|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|srcDevice_hostname|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|user_username|


