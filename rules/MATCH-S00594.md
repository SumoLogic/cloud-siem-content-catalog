# [Rules](README.md): Alibaba ActionTrail KMS Activity

## Description
Alibaba KMS is an encryption and key management web service.  Besides encrypting and decrypting data, users and administrators can use this service to create keys, manage keys etc.  This signal indicates activity that enables and disables keys explicitly.  This activity has been surveyed to be a low volume event and could be considered suspicious given other activity involving the entity.  Additionally, monitoring for these events is required to achieve certain industry audit compliance.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Unknown/Other|
|Apply Risk to Entities|user_username, srcDevice_ip|
|Signal Name|Alibaba ActionTrail KMS Activity|
|Summary Expression|User: {{user_username}} from source IP: {{srcDevice_ip}} performed a {{action}} action|
|Score/Severity|Static: 1|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0006, _mitreAttackTechnique:T1552, _mitreAttackTechnique:T1552.004, _mitreAttackTechnique:T1552.005|
## Vendors and Products
- [Alibaba - ActionTrail](../products/79055042-52c8-4998-b201-bd2cd2dbca1f.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|action|
|Normalized Schema|listMatches|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|user_username|


