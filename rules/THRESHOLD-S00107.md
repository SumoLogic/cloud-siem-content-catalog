# [Rules](README.md): AWS Instance Discovery

## Description
Detects various describe and/or list commands used for an instance in AWS.

## Additional Details
|Detail|Value|
|----|----|
|Type|Threshold|
|Category|Discovery|
|Apply Risk to Entities|srcDevice_ip, device_ip, user_username|
|Signal Name|AWS Instance Discovery|
|Summary Expression|AWS Instance Discovery Detected with IP: {{srcDevice_ip}} and User: {{user_username}}|
|Threshold Count|5|
|Threshold Window|5m|
|Score/Severity|Static: 1|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0007, _mitreAttackTechnique:T1526|
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


