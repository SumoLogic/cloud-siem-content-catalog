# [Rules](README.md): GitHub - First Seen Application Interacting with API

## Description
Detects new application usage of the GitHub API. New applications utilizing the API may be routine, however this may also reveal malicious applications utilzing the API. This detection was developed utilizing GitHub Enterprise Audit logging. Refer to https://help.sumologic.com/docs/integrations/app-development/github/#collecting-logs-for-github for instructions on ingesting GitHub Enterprise Audit logs.

## Additional Details
|Detail|Value|
|----|----|
|Type|First Seen|
|Category|Credential Access|
|Apply Risk to Entities|user_username, repository|
|Signal Name|GitHub - First Seen Application Interacting with API: {{application}}|
|Summary Expression|Application: {{application}}  observed performing action: {{normalizedAction}}  on behalf of user: {{user_username}}|
|Retention Window|7776000000|
|Baseline Window|2592000000|
|Baseline Type|GLOBAL|
|Score/Severity|Static: 2|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0006|
## Vendors and Products
- [Github - GitHub Enterprise Audit](../products/e3c8bd8b-6ed8-4332-944d-d0f5dfc462df.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|action|
|Normalized Schema|application|
|Normalized Schema|metadata_product|
|Normalized Schema|repository|
|Normalized Schema|user_username|


