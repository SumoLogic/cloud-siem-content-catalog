# [Rules](README.md): GitHub - Outlier in Distinct User Agent Strings by User

## Description
Detects an outlier in the number of distinct user agent strings for a GitHub user. Unusual user agent strings for a user account could indicate account takeover. This detection was developed utilizing GitHub Enterprise Audit logging. Refer to https://help.sumologic.com/docs/integrations/app-development/github/#collecting-logs-for-github for instructions on ingesting GitHub Enterprise Audit logs.

## Additional Details
|Detail|Value|
|----|----|
|Type|Outlier|
|Category|Initial Access|
|Apply Risk to Entities|user_username|
|Signal Name|GitHub - Outlier in Distinct User Agent Strings for {{user_username}}|
|Summary Expression|Unusual distinct user agent string by {{user_username}}|
|Retention Window|7776000000|
|Baseline Window|2592000000|
|Standard Deviation Threshold|2|
|Floor Value|4|
|Score/Severity|Static: 2|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0001, _mitreAttackTactic:TA0003, _mitreAttackTactic:TA0004, _mitreAttackTechnique:T1078|
## Vendors and Products
- [Github - GitHub Enterprise Audit](../products/e3c8bd8b-6ed8-4332-944d-d0f5dfc462df.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|http_userAgent|
|Normalized Schema|metadata_product|
|Normalized Schema|user_username|


