# [Rules](README.md): GCP Image Creation

## Description
Detects the creation of an image in GCP.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Defense Evasion|
|Apply Risk to Entities|srcDevice_ip, user_username|
|Signal Name|GCP Image Creation|
|Summary Expression|GCP Image Creation Detected: {{action}}  with IP: {{srcDevice_ip}} and User: {{user_username}}|
|Score/Severity|Static: 0|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTechnique:T1612, _mitreAttackTactic:TA0005|
## Vendors and Products
- [Google - Google Cloud Platform](../products/dcc85cfc-a698-4d09-87de-f2c723f3ad07.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|action|
|Normalized Schema|listMatches|
|Normalized Schema|lower|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|user_username|


