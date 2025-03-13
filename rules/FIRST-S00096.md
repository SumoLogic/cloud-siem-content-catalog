# [Rules](README.md): Azure DevOps - First Seen User Modifying Release Pipeline

## Description
Context:
Creation or modification of release pipelines provide opportunities for the attacker to introduce malicious code into the release process.

Detection:
This detection monitors for users modifying a release pipeline for the first time after the baseline period (by default, 90 days).

Recommended Actions:
Investigate the pipeline that has been created for malicious content and the user account activity for signs of account compromise or insider threat activity.

Tuning Recommendations:
Maintain a match list of users known and approved to create Azure DevOps pipeline and add it as a tuning expression for the rule.

Credits:
This detection is based on the Azure Sentinel ADOPipelineModifiedbyNewUser.yaml rule.

## Additional Details
|Detail|Value|
|----|----|
|Type|First Seen|
|Category|Unknown/Other|
|Apply Risk to Entities|user_username|
|Signal Name|Azure DevOps - First Seen User Modifying Release Pipeline|
|Summary Expression|First observation of User: {{user_username}} modifying an Azure DevOps Release Pipeline|
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


