# [Rules](README.md): Azure DevOps - First Seen Pull Request Policy Bypassed

## Description
Context:
An attacker can use pull request bypasses to introduce malicious code into production by circumventing normal review processes.

Detection:
This detection monitors for when a user performs a pull request bypass for the first time.

Tuning Recommendations:
If there is a known use case for pull request bypasses (emergency updates, lack of available review staff, etc.), add a tuning expression to exclude the user from the detection.

Recommended Actions:
Determine whether the pull request bypass was expected.
Investigate the user who performed the pull request bypass for indications of account compromise or other insider threat activity.

Credits:
This detection is based on the Azure Sentinel AzDOHistoricPrPolicyBypassing.yaml rule.

## Additional Details
|Detail|Value|
|----|----|
|Type|First Seen|
|Category|Unknown/Other|
|Apply Risk to Entities|user_username|
|Signal Name|Azure DevOps - First Seen Pull Request Policy Bypassed|
|Summary Expression|User: {{user_username}} has been observed bypassing policy|
|Retention Window|7776000000|
|Baseline Window|2592000000|
|Baseline Type|GLOBAL|
|Score/Severity|Static: 4|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTechnique:T1098.001|
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


