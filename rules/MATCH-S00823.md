# [Rules](README.md): Exposed AWS SQS Queue Created

## Description
An AWS Simple Queue Service (SQS) can be created with a custom access policy, this signal triggers when a policy is applied to an SQS queue which allows global access from the internet with an IP range of 0.0.0.0/32 (all)

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Collection|
|Apply Risk to Entities|user_username|
|Signal Name|Exposed AWS SQS Queue Created|
|Summary Expression|{{user_username}} has applied an access policy to an AWS Simple Queue Service (SQS) with an IP range that allows global access|
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
|Normalized Schema|application|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|user_username|


