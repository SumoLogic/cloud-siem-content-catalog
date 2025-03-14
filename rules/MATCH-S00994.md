# [Rules](README.md): Azure DevOps - Member Added to Sensitive Group

## Description
Context:
Any changes to administrative groups such as Project Administrators or Project Collection Administrators is noteworthy as they result in the user having a broad set of permissions.

Detection:
This detection monitors for changes to the following groups: Project Administrators, Project Collection Administrators, Project Collection Service Accounts, Build Administrator

Recommended Actions:
Determine whether the group modification was an approved change (for example, look for a change control ticket).
Investigate the user who modified the group for indications of account compromise or other insider threat activity.

Tuning Recommendations:
n/a

Credits:
This detection is based on the Azure Sentinel NewPAPCAPCASaddedtoADO.yaml rule.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Unknown/Other|
|Apply Risk to Entities|user_username|
|Signal Name|Azure DevOps - Member Added to Sensitive Group|
|Summary Expression|User: {{user_username}} added Member to a Sensitive Azure DevOps Group|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTechnique:T1078.004|
## Vendors and Products
- [Microsoft - Azure DevOps Auditing](../products/c3b61ddb-4d2d-497c-b873-28938036b67b.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|changeTarget|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|user_username|


