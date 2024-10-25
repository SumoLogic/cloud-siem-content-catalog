# [Rules](README.md): AWS Bedrock Model Invocation Logging Configuration Change Observed

## Description
An AWS Bedrock Model invocation logging configuration change was observed. Ensure that this activity is expected and authorized. Take a look at the full event details, particularly the requestParameters.loggingConfig* fields in order to see what specific configuration values were changed. Telemetry and logging configuration changes should be a relatively rare occurrence in the environment.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Defense Evasion|
|Apply Risk to Entities|user_username|
|Signal Name|AWS Bedrock Model Invocation Logging Configuration Change Observed by {{user_username}}|
|Summary Expression|AWS Bedrock Model Invocation Logging Configuration Change Observed by {{user_username}} from IP {{device_ip}}|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0005, _mitreAttackTechnique:T1562.008|
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


