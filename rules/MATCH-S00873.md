# [Rules](README.md): AWS EKS Cluster Configuration Updated

## Description
AWS EKS clusters contain various configuration options, including for which IP addresses can access the cluster API. Ensure that this change is authorized and expected.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Defense Evasion|
|Apply Risk to Entities|user_username|
|Signal Name|{{user_username}} has updated an AWS EKS Cluster Configuration|
|Summary Expression|An AWS EKS Cluster configuration has been updated by {{user_username}} from the IP address of {{srcDevice_ip}}|
|Score/Severity|Static: 4|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0005, _mitreAttackTechnique:T1078.004|
## Vendors and Products
- [Amazon AWS - CloudTrail](../products/033624b0-218e-4dcb-b93f-0f1fb1806c56.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|action|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|user_username|


