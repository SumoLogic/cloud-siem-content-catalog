# [Rules](README.md): Azure DevOps - Pipeline Retention Settings Reduced

## Description
Context:
AzureDevOps retains items such as run records and produced artifacts for a configurable amount of time. An attacker can cover up evidence of malicious activity by reducing the retention time.

Detection:
This detection monitors for any reduction in the pipeline retention settings.

Tuning Recommendations:
n/a

Recommended Actions:
Determine whether the retention setting reduction was an approved change (for example, look for a change control ticket).
Investigate the user who reduced the retention setting for indications of account compromise or insider threat activity.

Credits:
This detection is based on the Azure Sentinel ADORetentionReduced.yaml rule.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Unknown/Other|
|Apply Risk to Entities|user_username|
|Signal Name|Azure DevOps - Pipeline Retention Settings Reduced by User: {{user_username}}|
|Summary Expression|User: {{user_username}}  has reduced the Pipeline Retention settings|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTechnique:T1564|
## Vendors and Products
- [Microsoft - Azure DevOps Auditing](../products/c3b61ddb-4d2d-497c-b873-28938036b67b.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|action|
|Direct from Record|fields['data.Data.NewValue']|
|Direct from Record|fields['data.Data.OldValue']|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|user_username|


