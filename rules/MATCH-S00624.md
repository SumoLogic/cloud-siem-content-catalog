# [Rules](README.md): GCP Audit IAM Custom Role Created or Modified

## Description
Detect when a custom role is created or modified.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Defense Evasion|
|Apply Risk to Entities|user_username, srcDevice_ip|
|Signal Name|GCP Audit IAM Custom Role Created or Modified|
|Summary Expression|User: {{user_username}} performed action: {{action}}|
|Score/Severity|Static: 1|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0003, _mitreAttackTactic:TA0004, _mitreAttackTechnique:T1098, _mitreAttackTechnique:T1098.001|
## Vendors and Products
- [Google - Google Cloud Platform](../products/dcc85cfc-a698-4d09-87de-f2c723f3ad07.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|action|
|Normalized Schema|listMatches|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|user_username|


