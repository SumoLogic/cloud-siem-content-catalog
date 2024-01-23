# [Rules](README.md): New Container Uploaded to AWS ECR

## Description
New Container Uploaded to AWS ECR

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Defense Evasion|
|Apply Risk to Entities|device_hostname, device_ip, user_username, srcDevice_ip|
|Signal Name|New Container Uploaded to AWS ECR|
|Summary Expression|Action: {{action}} performed by user: {{user_username}} from IP: {{srcDevice_ip}}|
|Score/Severity|Static: 2|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTechnique:T1578, _mitreAttackTechnique:T1610, _mitreAttackTechnique:T1578.002, _mitreAttackTactic:TA0005|
## Vendors and Products
- [Amazon AWS - CloudTrail](../products/033624b0-218e-4dcb-b93f-0f1fb1806c56.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Direct from Record|fields['userIdentity.type']|
|Normalized Schema|http_userAgent|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|user_username|


