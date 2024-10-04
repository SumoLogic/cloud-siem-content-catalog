# [Rules](README.md): AWS Bedrock Agent Created

## Description
This rule detects when an AWS Bedrock Agent has been created in the environment. Bedrock Agents can be configured with various parameters to build AI applications. Take a look at the "responseElements.agent.agentName" field to see the name of the agent being created. Ensure that the user creating the agent is authorized to develop AI applications within the environment.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Discovery|
|Apply Risk to Entities|user_username|
|Signal Name|AWS Bedrock Agent Created by {{user_username}}|
|Summary Expression|AWS Bedrock Agent Created by {{user_username}} with the role {{user_username_role}}|
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
|Normalized Schema|cloud_provider|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|user_username|


