# [Rules](README.md): First Seen AWS SSM RunShellScript SendCommand From User

## Description
AWS SSM (Simple Systems Manager) can be used to manage systems and configurations, however, it can also be abused by threat actors to run various shell scripts on EC2 instances.

## Additional Details
|Detail|Value|
|----|----|
|Type|First Seen|
|Category|Execution|
|Apply Risk to Entities|user_username|
|Signal Name|First Seen AWS SSM RunShellScript SendCommand From User|
|Summary Expression|The user {{user_username}} has issued a RunShellScript command to an EC2 instance for the first time since the baseline period.|
|Retention Window|7776000000|
|Baseline Window|1296000000|
|Baseline Type|GLOBAL|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0002, _mitreAttackTechnique:T1204, _mitreAttackTechnique:T1651|
## Vendors and Products
- [Amazon AWS - CloudTrail](../products/033624b0-218e-4dcb-b93f-0f1fb1806c56.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|action|
|Normalized Schema|application|
|Direct from Record|fields["requestParameters.documentName"]|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|user_username|
|Normalized Schema|user_username_role|


