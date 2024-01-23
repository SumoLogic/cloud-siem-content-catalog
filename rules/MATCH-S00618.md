# [Rules](README.md): GCP Bucket Enumerated

## Description
Detects when a service account lists out GCS buckets.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Discovery|
|Apply Risk to Entities|user_username, srcDevice_ip|
|Signal Name|GCP Bucket Enumerated|
|Summary Expression|User: {{user_username}} performed action: {{action}}|
|Score/Severity|Static: 2|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0007, _mitreAttackTechnique:T1526, _mitreAttackTechnique:T1069, _mitreAttackTechnique:T1087, _mitreAttackTechnique:T1087.004, _mitreAttackTechnique:T1069.003|
## Vendors and Products
- [Google - Google Cloud Platform](../products/dcc85cfc-a698-4d09-87de-f2c723f3ad07.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|action|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|user_username|


