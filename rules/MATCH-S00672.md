# [Rules](README.md): AWS Config Recorder Stopped

## Description
Detects the AWS Config StopConfigurationRecorder API action. StopConfigurationRecorder stops recording configurations of the AWS resources you have selected to record in your AWS account.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Defense Evasion|
|Apply Risk to Entities|device_ip, user_username, srcDevice_ip, device_hostname, srcDevice_hostname|
|Signal Name|AWS Config Recorder Stopped|
|Summary Expression|{{action}} performed by user: {{user_username}}|
|Score/Severity|Static: 6|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTechnique:T1562, _mitreAttackTactic:TA0005, _mitreAttackTechnique:T1562.008, _mitreAttackTechnique:T1562.001|
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


