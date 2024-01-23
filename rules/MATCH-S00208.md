# [Rules](README.md): AWS CloudTrail - EC2 Access Key Action Detected

## Description
Actions observed that create, import and delete access keys to EC2 could indicate an advisary is taking action on their objective to extend or otherwise manipulate access to EC2 instance(s).

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Execution|
|Apply Risk to Entities|device_ip, user_username|
|Signal Name|AWS CloudTrail - EC2 Access Key Action Detected {{action}}|
|Summary Expression|{{action}} performed by user: {{user_username}} with role: {{user_username_role}} on target: {{changeTarget}}|
|Score/Severity|Static: 2|
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
|Normalized Schema|device_ip|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|user_username|


