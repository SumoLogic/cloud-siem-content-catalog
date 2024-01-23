# [Rules](README.md): AWS CloudTrail - sensitive activity in KMS

## Description
AWS KMS is an encryption and key management web service.  Besides encrypting and decrypting data, users and administrators can use this service to create keys, manage keys etc.  This signal indicates activity that enables and disables keys explicitly.  This activity has been surveyed to be a low volume event and could be considered suspicious given other activity involving the entity.  Additionally, monitoring for these events is required to achieve certain industry audit compliance.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Execution|
|Apply Risk to Entities|device_hostname, device_ip, user_username, srcDevice_ip|
|Signal Name|AWS CloudTrail - Sensitive activity in KMS {{metadata_deviceEventId}}|
|Summary Expression|{{action}} performed by user: {{user_username}}|
|Score/Severity|Static: 1|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0006, _mitreAttackTechnique:T1552, _mitreAttackTechnique:T1552.004, _mitreAttackTechnique:T1552.005|
## Vendors and Products
- [Amazon AWS - CloudTrail](../products/033624b0-218e-4dcb-b93f-0f1fb1806c56.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|listMatches|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|user_username|


