# [Rules](README.md): Azure DevOps - First Seen User Creating Agent Pool

## Description
Context:
Azure DevOps (ADO) Agent Pools are a key resource. Hosted or self-hosted pools can be created for use in the DevOps pipeline. An attacker with ADO access allowing for pool creation, may create agent pools for malicious use.

Detection:
This detection monitors for new users creating an agent pool. This user has not been observed creating agent pools during the baseline period and may be a new admin or involved in suspicious account activity.

Recommended Actions:
Investigate the account observed creating the new agent pool for signs of account compromise or insider threat activity.

Tuning Recommendations:
Create a tuning expression with a list of admin user_username values that should be excluded from detection if they were not in the baseline.

## Additional Details
|Detail|Value|
|----|----|
|Type|First Seen|
|Category|Defense Evasion|
|Apply Risk to Entities|user_username|
|Signal Name|First Seen - User Creating New Agent Pool|
|Summary Expression|User: {{user_username}}  has been observed creating a new Azure DevOps Agent Pool|
|Retention Window|7776000000|
|Baseline Window|2592000000|
|Baseline Type|GLOBAL|
|Score/Severity|Static: 2|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTechnique:T1578.002, _mitreAttackTactic:TA0005|
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


