# [Rules](README.md): SSH Keys Added to EC2 Instance

## Description
A set of SSH keys has been added to an AWS EC2 instance.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Persistence|
|Apply Risk to Entities|user_username|
|Signal Name|SSH Keys Added to EC2 Instance|
|Summary Expression|{{user_username}} using the IP address {{device_ip}} has added an SSH key to an EC2 Instance.|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0003, _mitreAttackTechnique:T1098.004, _mitreAttackTechnique:T1098.001|
## Vendors and Products
- [Amazon AWS - CloudTrail](../products/033624b0-218e-4dcb-b93f-0f1fb1806c56.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|action|
|Direct from Record|fields["responseElements.success"]|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|user_username|


