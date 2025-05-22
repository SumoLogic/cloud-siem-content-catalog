# [Rules](README.md): First Seen User Enumerating Custom AWS Bedrock Models

## Description
[Disabled by Default] Detection of a user account's first enumeration of custom AWS Bedrock models via ListCustomModels API. Verify the user is authorized for AWS Bedrock access. The http_userAgent field indicates whether a browser or CLI tool was used. This rule is disabled by default due to potential high volume of alerts, particularly from service accounts. Before enabling, consider excluding authorized users and service accounts (such as CNAPP monitoring accounts with timestamp-based usernames) through rule tuning expressions.

## Additional Details
|Detail|Value|
|----|----|
|Type|First Seen|
|Category|Discovery|
|Apply Risk to Entities|user_username|
|Signal Name|First Seen User: {{user_username}} Enumerating Custom AWS Bedrock Models|
|Summary Expression|First Seen User: {{user_username}} observed as enumerating AWS custom Bedrock models since the baseline period.|
|Retention Window|7776000000|
|Baseline Window|2592000000|
|Baseline Type|GLOBAL|
|Score/Severity|Static: 1|
|Enabled by Default|False|
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


