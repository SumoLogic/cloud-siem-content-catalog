# [Rules](README.md): First Seen S3 Bucket ACL Enumeration by User

## Description
Threat actors may collect information from AWS S3 buckets, including enumeration of access they have to such resources.

## Additional Details
|Detail|Value|
|----|----|
|Type|First Seen|
|Category|Collection|
|Apply Risk to Entities|user_username|
|Signal Name|First Seen S3 Bucket ACL Enumeration by User|
|Summary Expression|{{user_username}} has enumerated an AWS S3 Bucket ACL for the first time since the baseline period.|
|Retention Window|7776000000|
|Baseline Window|3024000000|
|Baseline Type|PER_ENTITY|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0009, _mitreAttackTechnique:T1530|
## Vendors and Products
- [Amazon AWS - CloudTrail](../products/033624b0-218e-4dcb-b93f-0f1fb1806c56.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|action|
|Direct from Record|fields["userIdentity.type"]|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|user_username|
|Normalized Schema|user_username_role|


