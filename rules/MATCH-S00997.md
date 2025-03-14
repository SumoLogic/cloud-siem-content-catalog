# [Rules](README.md): Azure DevOps - Browser Observed in Personal Access Token (PAT) Use

## Description
Context:
Personal Access Tokens (PATs) can be used to authenticate into Azure DevOps. PATs are intended to be used for authenticating automated access to Azure rather than for interactive use cases. Observing PAT authentication in interactive use cases could indicate that the PAT was stolen.

Detection:
This detection monitors for the use of a PAT for authentication from a User Agent String indicating a web browser.

Recommended Actions:
Investigate the user account associated with the Personal Access Token and the user’s workstation for signs of compromise.

Tuning Recommendations:
If your organization has known legitimate use cases for PAT authentication with a browser, add a tuning expression specific to the known use case. For example, you may tune out specific users, user agent strings or IP addresses as known use cases.

Credits:
This detection is based on the Azure Sentinel ADOPATUsedWithBrowser.yaml rule.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Credential Access|
|Apply Risk to Entities|user_username|
|Signal Name|Azure DevOps - Browser Observed in Personal Access Token (PAT) Use by {{user_username}}|
|Summary Expression|User: {{user_username}} has been observed using a PAT with a browser|
|Score/Severity|Static: 5|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTechnique:T1528, _mitreAttackTactic:TA0006|
## Vendors and Products
- [Microsoft - Azure DevOps Auditing](../products/c3b61ddb-4d2d-497c-b873-28938036b67b.md)


## Fields Used

|Origin|Field|
|----|----|
|Direct from Record|fields['data.AuthenticationMechanism']|
|Normalized Schema|http_userAgent|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|user_username|


