# [Rules](README.md): AWS Bedrock Model Invocation Denied for User

## Description
A user has attempted to invoke a model via AWS Bedrock for which access was denied due to a permission issue. This event can be a normal occurrence for a user who has not been provisioned the proper IAM resources for AWS Bedrock. However, it could also be a malicious attempt at running a particular model via AWS Bedrock. Take a look at the username, IP address, role type, role and model via the fields["requestParameters.modelId"] field.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Discovery|
|Apply Risk to Entities|user_username|
|Signal Name|AWS Bedrock Model Invocation Denied for {{user_username}}|
|Summary Expression|AWS Bedrock Model Invocation Denied for {{user_username}}|
|Score/Severity|Static: 2|
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
|Direct from Record|fields["errorCode"]|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|user_username|


