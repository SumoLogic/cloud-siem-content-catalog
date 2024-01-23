# [Rules](README.md): GCP Instance Discovery

## Description
Detects various discovery commands used for instances in GCP.

## Additional Details
|Detail|Value|
|----|----|
|Type|Threshold|
|Category|Discovery|
|Apply Risk to Entities|srcDevice_ip, user_username|
|Signal Name|GCP Instance Discovery|
|Summary Expression|GCP Instance Discovery Detected with IP: {{srcDevice_ip}} and User: {{user_username}}|
|Threshold Count|3|
|Threshold Window|5m|
|Score/Severity|Static: 1|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0007, _mitreAttackTechnique:T1526|
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


