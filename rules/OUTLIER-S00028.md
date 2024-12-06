# [Rules](README.md): GitHub - Outlier in Removal Actions by User

## Description
Detects a higher than usual number of removal actions undertaken by a user. This detection has a broad scope to detect any unusual number of destroy, delete, or remove actions undertaken by a user to help detect a range of different potential destructive activities in GitHub.

## Additional Details
|Detail|Value|
|----|----|
|Type|Outlier|
|Category|Impact|
|Apply Risk to Entities|user_username|
|Signal Name|GitHub - {{user_username}}  has Performed an Unusual Number of Removal Actions|
|Summary Expression|An unusual number of remove actions was performed by the user: {{user_username}}|
|Retention Window|7776000000|
|Baseline Window|2592000000|
|Standard Deviation Threshold|3|
|Floor Value|8|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0040, _mitreAttackTechnique:T1485|
## Vendors and Products
- [Github - GitHub Enterprise Audit](../products/e3c8bd8b-6ed8-4332-944d-d0f5dfc462df.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|metadata_product|
|Normalized Schema|normalizedAction|
|Normalized Schema|user_username|


