# [Rules](README.md): AWS CloudTrail - IAM Policy Applied

## Description
A policy was attached to a user, group, or role. By default, IAM denies all access to all services for users, and policies must be applied to grant access to AWS services and resources. This signal could indicate a policy is granting additional access within your cloud environment.

## Additional Details
|Detail|Value|
|----|----|
|Type|Match|
|Category|Privilege Escalation|
|Apply Risk to Entities|device_ip, user_username|
|Signal Name|AWS CloudTrail - IAM Policy Applied|
|Summary Expression|{{action}} performed by user: {{user_username}}|
|Score/Severity|Static: 1|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0004, _mitreAttackTactic:TA0005, _mitreAttackTechnique:T1078, _mitreAttackTechnique:T1078.004|
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


