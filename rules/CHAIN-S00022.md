# [Rules](README.md): Azure DevOps - Agent Pool Created and Deleted within a Short Period

## Description
Context:
An attacker may create Azure DevOps Agent Pools for malicious activity that are separate from an organization’s pools.

Detection:
This detection monitors for the creation and deletion of Agent Pools within 5 days by the same user, with the intent of finding Agent Pools active for short durations.

Recommended Actions:
If an alert occurs, investigate the actions taken by the account to determine if this is normal operation of deleting pools or if this suspicious activity. 

Tuning Recommendations: 
If necessary, add a tuning expression for users who frequently create and delete agent pools within the time period specified.
If necessary, adjust the "within" time period to better represent what is considered a short time period in your organization. Note that 5 days is the maximum time period you can specify for a chain rules.

Credits: 
This rule is loosely based on the Azure Sentinel ADOAgentPoolCreatedDeleted.yaml detection.


## Additional Details
|Detail|Value|
|----|----|
|Type|Chain|
|Category|Defense Evasion|
|Apply Risk to Entities|user_username|
|Signal Name|Azure DevOps - Agent Pool Created and Deleted within a Short Period|
|Summary Expression|User: {{user_username}}  has created and deleted an agent pool in a short period of time|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTechnique:T1578, _mitreAttackTactic:TA0005|
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


