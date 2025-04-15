# [Rules](README.md): GitHub - Organization Transfer

## Description
Detects transfers of an organization to another enterprise This is a sensitive activity that should be monitored to ensure organizations and their repositories are not being transferred without proper authorization. This detection was developed utilizing GitHub Enterprise Audit logging. Refer to https://help.sumologic.com/docs/integrations/app-development/github/#collecting-logs-for-github for instructions on ingesting GitHub Enterprise Audit logs.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Lateral Movement|
|Apply Risk to Entities|user_username|
|Signal Name|GitHub - {{user_username}} Transferred an Organization to Another Enterprise|
|Summary Expression|{{user_username}} transferred the {{fields['org']}}|
|Score/Severity|Static: 5|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0008, _mitreAttackTechnique:T1537, _mitreAttackTactic:TA0010|
## Vendors and Products
- [Github - GitHub Enterprise Audit](../products/e3c8bd8b-6ed8-4332-944d-d0f5dfc462df.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|action|
|Normalized Schema|metadata_product|
|Normalized Schema|user_username|


