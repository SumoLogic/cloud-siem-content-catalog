# [Rules](README.md): AWS Instance Creation

## Description
Detects the creation of an instance in AWS.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Defense Evasion|
|Apply Risk to Entities|srcDevice_ip, device_ip, user_username|
|Signal Name|AWS Instance Creation|
|Summary Expression|AWS Instance Creation Detected with IP: {{srcDevice_ip}} and User: {{user_username}}|
|Score/Severity|Static: 0|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTechnique:T1578, _mitreAttackTechnique:T1578.002, _mitreAttackTactic:TA0005|
## Vendors and Products
- [Amazon AWS - CloudTrail](../products/033624b0-218e-4dcb-b93f-0f1fb1806c56.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|action|
|Normalized Schema|device_ip|
|Normalized Schema|listMatches|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|user_username|


