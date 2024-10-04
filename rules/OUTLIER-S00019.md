# [Rules](README.md): Outlier in AWS Bedrock API Calls from User

## Description
An outlier in the number of API calls made to AWS Bedrock from a user within an hour time period was observed. These events may be part of normal Bedrock operations or may be indicative of enumeration/discovery attempts. Observe the username, role, user agent and source IP to confirm whether this activity is expected. If this signal is triggering frequently, consider excluding certain authorized users via tuning expression.

## Additional Details
|Detail|Value|
|----|----|
|Type|Outlier|
|Category|Discovery|
|Apply Risk to Entities|user_username|
|Signal Name|Outlier in AWS Bedrock API Calls from User: {{user_username}}|
|Summary Expression|Outlier in AWS Bedrock API Calls from User: {{user_username}}|
|Retention Window|7776000000|
|Baseline Window|2592000000|
|Standard Deviation Threshold|2|
|Floor Value|15|
|Score/Severity|Static: 1|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTechnique:T1526, _mitreAttackTactic:TA0007|
## Vendors and Products
- [Amazon AWS - CloudTrail](../products/033624b0-218e-4dcb-b93f-0f1fb1806c56.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|application|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|user_username|


