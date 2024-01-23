# [Rules](README.md): AWS CloudTrail - Customer Master Key Disabled or Scheduled for Deletion

## Description
The AWS Key Management Service (KMS) can be used to generate key pairs for encrypting and decrypting your data. Disabling or deleting keys can come with heavy destructive consequences as data encrypted with those keys cannot be decrypted. AWS forces users to either disable keys allowing them to be re-enabled at a later time or users must schedule a key deletion at a later time if the keys absolutely must be removed. The default time for scheduling a key deletion is 30 days.

## Additional Details
|Detail|Value|
|----|----|
|Type|Match|
|Category|Defense Evasion|
|Apply Risk to Entities|device_hostname, device_ip, user_username, srcDevice_ip|
|Signal Name|AWS CloudTrail - Customer Master Key Disabled or Scheduled for Deletion|
|Summary Expression|{{action}} performed on Customer Master Key by user: {{user_username}}|
|Score/Severity|Static: 1|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0006, _mitreAttackTechnique:T1552, _mitreAttackTechnique:T1552.004, _mitreAttackTechnique:T1552.005|
## Vendors and Products
- [Amazon AWS - CloudTrail](../products/033624b0-218e-4dcb-b93f-0f1fb1806c56.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|action|
|Normalized Schema|application|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|user_username|


