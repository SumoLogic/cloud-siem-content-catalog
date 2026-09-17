# [Rules](README.md): First Seen AWS API Gateway Enumeration by User

## Description
Threat actors may collect information from AWS API Gateway, including enumeration of access they have to such resources.

## Additional Details
|Detail|Value|
|----|----|
|Type|First Seen|
|Category|Collection|
|Apply Risk to Entities|user_username|
|Signal Name|First Seen AWS API Gateway Enumeration By User|
|Summary Expression|{{user_username}} has enumerated an AWS API Gateway resources for the first time since the baseline period.|
|Retention Window|5184000000|
|Baseline Window|1209600000|
|Baseline Type|GLOBAL|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0009, _mitreAttackTechnique:T1530|
## Vendors and Products
- [Amazon AWS - CloudTrail](../products/033624b0-218e-4dcb-b93f-0f1fb1806c56.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|application|
|Direct from Record|fields["userIdentity.type"]|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|user_username|
|Normalized Schema|user_username_role|


