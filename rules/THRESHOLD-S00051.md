# [Rules](README.md): AWS CloudTrail - IAM User Generating AccessDenied Errors Across Multiple Actions

## Description
An IAM account sent multiple requests to perform a wide distinct number of AWS actions in a short time frame while receiving the error code AccessDenied. This could indicate an account attempting to enumerate their access across the AWS account.

## Additional Details
|Detail|Value|
|----|----|
|Type|Threshold|
|Category|Initial Access|
|Apply Risk to Entities|device_hostname, device_ip, user_username, srcDevice_ip|
|Signal Name|AWS CloudTrail - IAM User Generating AccessDenied Errors Across Multiple Actions|
|Summary Expression|AWS API Call attempts denied by user: {{user_username}} 10+ times|
|Threshold Count|10|
|Threshold Window|30m|
|Score/Severity|Static: 1|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0006, _mitreAttackTechnique:T1552, _mitreAttackTechnique:T1552.005|
## Vendors and Products
- [Amazon AWS - CloudTrail](../products/033624b0-218e-4dcb-b93f-0f1fb1806c56.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Direct from Record|fields['errorCode']|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|user_username|


