# [Rules](README.md): AWS Bedrock - Rapid Guardrail Interventions

## Description
Detection:
This rule triggers when 10 or more Bedrock Guardrail interventions occur within 60 seconds for a user. It monitors CloudWatch logs where stopReason equals 'guardrail_intervened', indicating the guardrail blocked model responses that violated content policies.

Scenario:
An attacker or unauthorized user may attempt to jailbreak Bedrock models by rapidly probing guardrail boundaries to find policy bypass techniques. High intervention rates indicate potential jailbreak attempts, unsanctioned model use, or automated attacks testing content filtering limits.

Recommended Actions:
Review user_username to identify the account generating interventions and verify their authorization to use Bedrock. Examine the CloudWatch logs to determine the nature of blocked prompts and assess whether this represents malicious jailbreak attempts or legitimate boundary testing.

Tuning Recommendations:
Adjust the threshold from 10 to a higher value if legitimate users frequently test guardrail boundaries during development or QA activities. Exclude known test accounts performing authorized red team exercises or model evaluation testing.

## Additional Details
|Detail|Value|
|----|----|
|Type|Threshold|
|Category|Unknown/Other|
|Apply Risk to Entities|user_username|
|Signal Name|AWS Bedrock - Rapid Guardrail Interventions|
|Summary Expression|Rapid AWS Bedrock Guardrail interventions have been triggered  for {{user_username}}|
|Threshold Count|10|
|Threshold Window|CUSTOM|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAtlasTactic:AML.TA0012, _mitreAtlasTechnique:AML.T0054|
## Vendors and Products
- [Amazon AWS - CloudWatch](../products/b57c366d-e6a5-4e61-b950-5686a902bc24.md)


## Fields Used

|Origin|Field|
|----|----|
|Direct from Record|fields["output.outputBodyJson.stopReason"]|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|user_username|


