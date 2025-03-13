# [Rules](README.md): Azure DevOps - Personal Access Token (PAT) Misuse Observed

## Description
Context:
Authentication to Azure DevOps via a Personal Access Token (PAT) is intended for particular use cases and should not be observed with all actions in Azure. This Alert detects whenever a PAT is used in ways that PATs are not normally used. If unusual PAT use is observed it potentially indicates the PAT was stolen by an attacker.

Detection:
This detection monitors for use of a Personal Access Token in conjunction with categories of action that aren’t normally associated with PAT authentication.

Recommended Actions:
Determine whether the PAT use is part of a known and approved use case.
Investigate the user whose PAT was used for indications of account compromise or other insider threat activity. 
Investigate the workstation of the user for indications of compromise.

Tuning Recommendations:
If your organization has known use cases, such as automation, that trigger this rule, add a tuning expression to exclude either the action or other distinguishing metadata such as the user.

Credits:
This detection is based on the Azure Sentinel AzDOPatSessionMisuse.yaml rule.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Unknown/Other|
|Apply Risk to Entities|user_username|
|Signal Name|Azure DevOps - Personal Access Token (PAT) Misuse Observed|
|Summary Expression|User: {{user_username}} Personal Access Token has been used suspiciously|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTechnique:T1496|
## Vendors and Products
- [Microsoft - Azure DevOps Auditing](../products/c3b61ddb-4d2d-497c-b873-28938036b67b.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|action|
|Direct from Record|fields['data.AuthenticationMechanism']|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|user_username|


