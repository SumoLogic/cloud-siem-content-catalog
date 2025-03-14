# [Rules](README.md): Azure DevOps - Pipeline Created and Deleted within a Short Period

## Description
Context:
An attacker may use a pipeline for malicious activity such as introducing malicious code into production or executing malicious code in an agent pool. The attacker likely will delete the pipeline after achieving their objectives in order to cover their tracks.

Detection:
This detection monitors for the creation and deletion of the same pipeline within a short period (by default, a day).

Recommended Actions:
Investigate whether the rapid creation and deletion of the pipeline was an expected activity. 
Review build artifacts resulting from the pipeline for malicious code. 
Investigate the user for indications of account compromise or insider threat activity.

Tuning Recommendations:
Adjust the time constraints of the rule from one day to one which aligns better to the practices in your organization. 
If there are known use cases for rapid creation and deletion of pipelines in your organization, add a tuning expression to exclude the distinguishing metadata such as the username.

Credits:
This detection is based on the Azure Sentinel AzDOPipelineCreatedDeletedOneDay.yaml rule.


## Additional Details
|Detail|Value|
|----|----|
|Type|Chain|
|Category|Unknown/Other|
|Apply Risk to Entities|user_username|
|Signal Name|Azure DevOps - Pipeline Created and Deleted within a Short Period|
|Summary Expression|User: {{user_username}} has been observed creating and deleting Azure DevOps Pipelines in a short period of time|
|Score/Severity|Static: 2|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTechnique:T1072|
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


