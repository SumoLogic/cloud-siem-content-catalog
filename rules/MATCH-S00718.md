# [Rules](README.md): AWS Image Modification

## Description
Detects the modification of an image in AWS.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Persistence|
|Apply Risk to Entities|srcDevice_ip, device_ip, user_username|
|Signal Name|AWS Image Modification|
|Summary Expression|AWS Image Modification Detected: {{action}} with IP: {{srcDevice_ip}} and User: {{user_username}}|
|Score/Severity|Static: 1|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTechnique:T1525, _mitreAttackTactic:TA0003|
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


