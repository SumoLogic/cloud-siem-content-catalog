# [Rules](README.md): Suspicious Lambda Function - IAM Policy Attached

## Description
A Lambda function has been used to assign an IAM role to a user, this may be potentially malicious or unexpected activity, particularly if Lambda is not used to assign IAM roles in the environment.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Privilege Escalation|
|Apply Risk to Entities|user_username|
|Signal Name|Suspicious Lambda Function - IAM Policy Attached|
|Summary Expression|The Lambda function {{user_username}}  has assigned an IAM policy to a user, please review the event details to determine if this is legitimate activity.|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0004, _mitreAttackTechnique:T1648|
## Vendors and Products
- [Amazon AWS - CloudTrail](../products/033624b0-218e-4dcb-b93f-0f1fb1806c56.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|action|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|user_username|


