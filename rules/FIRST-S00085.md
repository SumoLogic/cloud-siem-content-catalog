# [Rules](README.md): First Seen Role Creating AWS Bedrock Agent

## Description
An AWS Bedrock Agent has been created in the environment by a Role seen for the first time since the baseline period. If this role is not expected in the environment and was not originally assigned IAM rights to Bedrock, this activity could be indicative of privilege escalation. Bedrock Agents can be configured with various parameters to build AI applications. Take a look at the "responseElements.agent.agentName" field to see the name of the agent being created. Ensure that the user creating the agent is authorized to develop AI applications within the environment.

## Additional Details
|Detail|Value|
|----|----|
|Type|First Seen|
|Category|Discovery|
|Apply Risk to Entities|user_username|
|Signal Name|First Seen Role Creating AWS Bedrock Agent: {{user_role}}|
|Summary Expression|{{user_username}} has created a Bedrock Agent with a role not seen since the baseline period: {{user_role}} from IP: {{device_ip}}|
|Retention Window|7776000000|
|Baseline Window|3024000000|
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
|Normalized Schema|cloud_provider|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|user_role|
|Normalized Schema|user_username|


