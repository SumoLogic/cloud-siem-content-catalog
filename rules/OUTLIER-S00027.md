# [Rules](README.md): GitHub - Outlier in Repository Cloning or Downloads

## Description
Detects an unusual number of repository clones for a user. Unusual repository cloning could indicate data exfiltration or discovery. This detection was developed utilizing GitHub Enterprise Audit logging. Refer to https://help.sumologic.com/docs/integrations/app-development/github/#collecting-logs-for-github for instructions on ingesting GitHub Enterprise Audit logs.

## Additional Details
|Detail|Value|
|----|----|
|Type|Outlier|
|Category|Discovery|
|Apply Risk to Entities|user_username|
|Signal Name|GitHub - Outlier in Repository Clones or Downloads by {{user_username}}|
|Summary Expression|{{user_username}} has cloned or downloaded an unusual number of repositories.|
|Retention Window|7776000000|
|Baseline Window|2592000000|
|Standard Deviation Threshold|3|
|Floor Value|5|
|Score/Severity|Static: 2|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0007, _mitreAttackTactic:TA0010|
## Vendors and Products
- [Github - GitHub Enterprise Audit](../products/e3c8bd8b-6ed8-4332-944d-d0f5dfc462df.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|action|
|Normalized Schema|metadata_product|
|Normalized Schema|user_username|


