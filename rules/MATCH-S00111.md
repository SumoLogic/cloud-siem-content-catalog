# [Rules](README.md): AWS CloudTrail - IAM CreateUser Action Observed

## Description
This signal fires for all observances of the CreateUser action in the IAM event source.  Creating AWS users is likely a benign, infrequent activity.  Hostile actors will create users to persist access.  Use this signal in context of other activity to determine intent.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Persistence|
|Apply Risk to Entities|device_hostname, device_ip, user_username, srcDevice_ip|
|Signal Name|AWS CloudTrail - IAM CreateUser Action Observed|
|Summary Expression|User {{changeTarget}} created by user: {{user_username}}|
|Score/Severity|Static: 2|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0003, _mitreAttackTechnique:T1136, _mitreAttackTechnique:T1136.003|
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


