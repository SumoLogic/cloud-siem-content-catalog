# [Rules](README.md): GitHub - Vulnerability Alerts

## Description
Detects vulnerability alerts created for a GitHub repository.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Resource Development|
|Apply Risk to Entities|repository|
|Signal Name|GitHub - Vulnerability Alert Open|
|Summary Expression|GitHub Security Advisory ID: {{fields['ghsa_id']}} detected on {{repository}} with Alert ID: {{fields['alert_number']}}|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTechnique:T1588, _mitreAttackTactic:TA0042|
## Vendors and Products
- [Github - GitHub Enterprise Audit](../products/e3c8bd8b-6ed8-4332-944d-d0f5dfc462df.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|action|
|Normalized Schema|metadata_product|
|Normalized Schema|repository|


