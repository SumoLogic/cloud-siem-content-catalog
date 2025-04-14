# [Rules](README.md): GitHub - PR Review Requirement Removed

## Description
Detects GitHub pull request review requirements being removed from a repository either via branch protection rule or ruleset. This detection was developed utilizing GitHub Enterprise Audit logging. Refer to https://help.sumologic.com/docs/integrations/app-development/github/#collecting-logs-for-github for instructions on ingesting GitHub Enterprise Audit logs.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Defense Evasion|
|Apply Risk to Entities|user_username, repository|
|Signal Name|GitHub - PR Review Requirements Removed on the {{repository}} Repository|
|Summary Expression|User {{user_username}}  removed pull request review requirements on the {{repository}} repository|
|Score/Severity|Static: 2|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0005, _mitreAttackTechnique:T1553, _mitreAttackTechnique:T1553.006|
## Vendors and Products
- [Github - GitHub Enterprise Audit](../products/e3c8bd8b-6ed8-4332-944d-d0f5dfc462df.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|action|
|Direct from Record|fields['required_approving_review_count']|
|Direct from Record|fields['ruleset_rules_updated.1.parameters.required_approving_review_count']|
|Normalized Schema|metadata_product|
|Normalized Schema|repository|
|Normalized Schema|user_username|


