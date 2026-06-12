# [Rules](README.md): AWS Bedrock - Privileged Permissions Granted

## Description
Detection:
This rule triggers when Bedrock IAM permissions are granted through: (1) attachment of managed policies (AmazonBedrockFullAccess, AmazonBedrockStudioFullAccess), (2) creation of policies containing Bedrock actions, or (3) inline policy assignments. It monitors high-risk actions including model invocation, AI agent creation, guardrail deletion, logging configuration changes, knowledge base creation, and provisioned throughput allocation.

Scenario:
An attacker with IAM permissions escalates privileges by granting Bedrock access to themselves or compromised roles, enabling model invocation, AI agent creation, guardrail bypass, logging deletion, data exfiltration via knowledge bases, or cryptomining through expensive compute resources. Legitimate Bedrock provisioning may require similar permissions, making this a potential indicator of either authorized activity or privilege escalation.

Recommended Actions:
Verify the permission grant aligns with authorized Bedrock provisioning by reviewing user_username, srcDevice_ip, and timing against normal business hours. For inline policies, review policyDocument for overly permissive actions (bedrock:* wildcards), then if unauthorized, detach the policy immediately, rotate credentials, and check CloudTrail for any Bedrock API calls using the newly granted permissions.

Tuning Recommendations:
The rule excludes AWS service-linked roles. Create match list 'authorized_bedrock_provisioning_accounts' for users or roles that regularly provision Bedrock permissions, and adjust monitored Bedrock actions based on your organization's risk tolerance.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Persistence|
|Apply Risk to Entities|user_username|
|Signal Name|AWS - Privileged Bedrock Permissions Granted via {{action}} by {{user_username}}|
|Summary Expression|Privileged AWS Bedrock permissions granted: {{action}} performed by {{user_username}}|
|Score/Severity|Static: 2|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTechnique:T1098.003, _mitreAttackTactic:TA0003|
## Vendors and Products
- [Amazon AWS - CloudTrail](../products/033624b0-218e-4dcb-b93f-0f1fb1806c56.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|action|
|Direct from Record|fields['requestParameters.policyArn']|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|user_username|
|Normalized Schema|user_username_role|


