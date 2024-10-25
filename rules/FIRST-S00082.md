# [Rules](README.md): First Seen User Enumerating AWS Bedrock Models

## Description
A first seen user was observed enumerating AWS Bedrock models via the ListFoundationModels API call. Ensure that the user performing the enumeration is authorized to work within AWS Bedrock. The http_userAgent field will contain the user agent used to perform this enumeration and will help determine whether a browser or CLI tool was used to perform this type of enumeration. Consider excluding service accounts and authorized users from this rule via a rule tuning expression if excessive signal activity is observed.

## Additional Details
|Detail|Value|
|----|----|
|Type|First Seen|
|Category|Discovery|
|Apply Risk to Entities|user_username|
|Signal Name|First Seen User: {{user_username}} Enumerating AWS Bedrock Models|
|Summary Expression|First Seen User: {{user_username}} observed as enumerating AWS Bedrock models since the baseline period.|
|Retention Window|7776000000|
|Baseline Window|2592000000|
|Baseline Type|GLOBAL|
|Score/Severity|Static: 1|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0007, _mitreAttackTechnique:T1526|
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


