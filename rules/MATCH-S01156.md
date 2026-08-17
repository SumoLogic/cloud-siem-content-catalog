# [Rules](README.md): Claude Admin or Platform API Key Created

## Description
Detection:
This rule triggers when a new Admin or Platform API key is created within a Claude organization.

Scenario:
An attacker who has gained administrative access to a Claude organization may create new Admin or Platform API keys to establish persistent access. These keys provide elevated privileges for organization management and API access, and could be used for ongoing data exfiltration or unauthorized resource usage without requiring the compromised user's credentials.

Recommended Actions:
Verify the key creation was authorized by reviewing user_username and the scopes granted, and cross-reference with change management tickets. If unauthorized, disable or delete the key immediately and investigate the creating account for signs of compromise.

Tuning Recommendations:
If specific service accounts are authorized to routinely create API keys (e.g., automated provisioning systems), create a match list to exclude them. Monitor for keys created with unusually broad scopes.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Persistence|
|Apply Risk to Entities|user_username|
|Signal Name|Claude {{action}} by {{user_username}}|
|Summary Expression|Claude {{action}} by {{user_username}} from IP {{device_ip}}|
|Score/Severity|Static: 2|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0003, _mitreAttackTechnique:T1098.001, _mitreAtlasTactic:AML.TA0006, _mitreAtlasTechnique:AML.T0012, _mitreAtlasTechnique:AML.T0091.000|
## Vendors and Products


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|action|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|user_username|


