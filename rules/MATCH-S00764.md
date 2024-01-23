# [Rules](README.md): AWS CloudTrail - S3 Bucket Public Access Block Disabled

## Description
Detects when GetPublicAccessBlock returns NoSuchPublicAccessBlockConfiguration, indicating the public access block has all values are set to false or the feature is disabled.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Collection|
|Apply Risk to Entities|srcDevice_ip, device_ip, user_username|
|Signal Name|AWS CloudTrail - An S3 Bucket Public Access Block is Disabled|
|Summary Expression|An S3 Bucket Public Access Block is Disabled. {{action}} command run by User: {{user_username}} with IP: {{srcDevice_ip}} User: {{user_username}}|
|Score/Severity|Static: 2|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0009, _mitreAttackTechnique:T1530|
## Vendors and Products
- [Amazon AWS - CloudTrail](../products/033624b0-218e-4dcb-b93f-0f1fb1806c56.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|action|
|Normalized Schema|device_ip|
|Direct from Record|fields['errorCode']|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|user_username|


