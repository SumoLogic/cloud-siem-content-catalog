# [Rules](README.md): Azure DevOps - First Seen User Modifying Build Variables

## Description
Context:
An attacker can modify a variable group to alter the execution of the build pipeline for malicious results.

Detection:
This detection monitors for a user modifying a variable group for the first time.

Recommended Actions:
Determine whether the variable group modification was a known change.
Investigate the user who reduced the retention setting for indications of account compromise or other insider threat activity.

Tuning Recommendations:
Maintain a match list of users known and approved to modify variable groups and add it as a tuning expression for the rule.

Credits:
This detection is based on the Azure Sentinel ADOVariableModifiedByNewUser.yaml rule.

## Additional Details
|Detail|Value|
|----|----|
|Type|First Seen|
|Category|Unknown/Other|
|Apply Risk to Entities|user_username|
|Signal Name|Azure DevOps - First Seen User Modifying Build Variables|
|Summary Expression|User: {{user_username}} has been observed modifying a Variable group|
|Retention Window|7776000000|
|Baseline Window|2592000000|
|Baseline Type|GLOBAL|
|Score/Severity|Static: 2|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTechnique:T1578.005|
## Vendors and Products
- [Microsoft - Azure DevOps Auditing](../products/c3b61ddb-4d2d-497c-b873-28938036b67b.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|action|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|user_username|


