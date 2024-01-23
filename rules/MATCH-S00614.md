# [Rules](README.md): GCP Audit KMS Activity

## Description
GCP KMS is an encryption and key management web service. Besides encrypting and decrypting data, users and administrators can use this service to create keys, manage keys etc. This signal indicates activity that enables and disables keys explicitly. This activity has been surveyed to be a low volume event and could be considered suspicious given other activity involving the entity. Additionally, monitoring for these events is required to achieve certain industry audit compliance.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Initial Access|
|Apply Risk to Entities|user_username, srcDevice_ip|
|Signal Name|GCP Audit KMS Activity|
|Summary Expression|User: {{user_username}} performed action: {{action}}|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0006, _mitreAttackTechnique:T1552, _mitreAttackTechnique:T1552.004, _mitreAttackTechnique:T1552.005|
## Vendors and Products
- [Google - Google Cloud Platform](../products/dcc85cfc-a698-4d09-87de-f2c723f3ad07.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|action|
|Normalized Schema|application|
|Normalized Schema|listMatches|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|user_username|


