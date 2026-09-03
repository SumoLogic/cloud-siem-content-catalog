# [Rules](README.md): Claude Organization IP Restriction Deleted

## Description
Detection:
This rule triggers when an IP restriction is deleted from a Claude organization, removing a network access control.

Scenario:
An attacker with administrative access may delete IP restrictions to allow access from unauthorized networks, expanding the attack surface. This could be a preparatory step before accessing the organization from an external network or enabling access for compromised credentials from outside the corporate network. IP restrictions are a critical perimeter control that limits which networks can interact with the Claude organization.

Recommended Actions:
Verify the IP restriction deletion was authorized by reviewing user_username and checking if it aligns with approved network access changes. If unauthorized, recreate the IP restriction immediately and investigate the acting user's account for signs of compromise.

Tuning Recommendations:
Create a match list of authorized administrators who manage network access policies. For organizations with frequent legitimate IP restriction changes due to dynamic network environments, consider correlating with other indicators before escalation.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Defense Evasion|
|Apply Risk to Entities|user_username|
|Signal Name|Claude Organization IP Restriction Deleted by {{user_username}}|
|Summary Expression|Claude Organization IP Restriction Deleted by {{user_username}} from IP {{device_ip}}|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0112, _mitreAttackTechnique:T1685, _mitreAtlasTactic:AML.TA0007, _mitreAtlasTechnique:AML.T0107|
## Vendors and Products
- [Anthropic - Claude Activity Logs](../products/8ad9c55c-1271-4e8a-a8ca-f1663051f4d1.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|action|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|user_username|


