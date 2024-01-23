# [Rules](README.md): Suspicious AWS Lambda Enumeration

## Description
Threat actors will attempt to enumerate various system settings in order to explore privilege escalation avenues or to locate potentially sensitive data.

## Additional Details
|Detail|Value|
|----|----|
|Type|Aggregation|
|Category|Discovery|
|Apply Risk to Entities|user_username|
|Signal Name|Suspicious AWS Lambda Enumeration|
|Summary Expression|{{user_username}} has recorded a number of AWS Lambda enumeration commands issued in rapid succession, indicating a potentially malicious system enumeration attempt.|
|Aggregation Window|T05M|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0007, _mitreAttackTechnique:T1526|
## Vendors and Products
- [Amazon AWS - CloudTrail](../products/033624b0-218e-4dcb-b93f-0f1fb1806c56.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|application|
|Normalized Schema|cmd_count|
|Direct from Record|fields["requestParameters.roleSessionName"]|
|Direct from Record|fields["userIdentity.type"]|
|Normalized Schema|lower|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|user_username|
|Normalized Schema|user_username_role|


