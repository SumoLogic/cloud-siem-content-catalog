# [Rules](README.md): First Seen AWS EKS API Call via CloudTrail from User

## Description
This rule looks for a first seen AWS EKS API call from a user since the baseline period.

## Additional Details
|Detail|Value|
|----|----|
|Type|First Seen|
|Category|Discovery|
|Apply Risk to Entities|user_username|
|Signal Name|First Seen AWS EKS API Call ({{action}})  via CloudTrail from User|
|Summary Expression|The user {{user_username}} has performed an operation on an EKS cluster for the first time since the baseline period.|
|Retention Window|7776000000|
|Baseline Window|1814400000|
|Baseline Type|PER_ENTITY|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0007, _mitreAttackTechnique:T1613|
## Vendors and Products
- [Amazon AWS - CloudTrail](../products/033624b0-218e-4dcb-b93f-0f1fb1806c56.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|action|
|Normalized Schema|application|
|Normalized Schema|cloud_provider|
|Direct from Record|fields["errorCode"]|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|user_username|


