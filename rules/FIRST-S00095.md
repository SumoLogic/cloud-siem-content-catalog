# [Rules](README.md): Azure DevOps - New Agent OS Added to Agent Pool

## Description
Context:
An attacker could add an agent to an agent pool for the purpose of running malicious code during pipeline execution.

Detection:
This detection monitors for the addition of an agent to an agent pool when the OS of the agent has not been observed in this pool during the baseline period.

Recommended Actions:
Investigate whether the addition of the agent was an expected activity.
Review build artifacts resulting from the pipeline for malicious code.
Review execution activity on the agent during pipeline execution.
Investigate the user for indications of account compromise or insider threat activity.

Tuning Recommendations:
Add tuning expressions to exclude known agent additions in which the agent has a distinct operating system from the pool baseline. The tuning expression could be based on metadata such as the user or the OS.

Credits:
This detection is based on the Azure Sentinel NewAgentAddedToPoolbyNewUserorofNewOS.yaml rule.

## Additional Details
|Detail|Value|
|----|----|
|Type|First Seen|
|Category|Unknown/Other|
|Apply Risk to Entities|user_username|
|Signal Name|Azure DevOps - New Agent OS added to Agent Pool|
|Summary Expression|User: {{user_username}} has added a new Agent OS to an Agent Pool that is previously unseen|
|Retention Window|7776000000|
|Baseline Window|2592000000|
|Baseline Type|GLOBAL|
|Score/Severity|Static: 2|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTechnique:T1053|
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


