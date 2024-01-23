# [Rules](README.md): Alibaba ActionTrail IAM CreateUser Observed

## Description
This signal fires for all observances of the CreateUser action in the IAM event source.  Creating Alibaba Cloud users is likely a benign, infrequent activity.  Hostile actors will create users to persist access.  Use this signal in context of other activity to determine intent.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Unknown/Other|
|Apply Risk to Entities|user_username, srcDevice_ip|
|Signal Name|Alibaba ActionTrail IAM CreateUser Observed|
|Summary Expression|User: {{user_username}} from source IP: {{srcDevice_ip}} created a user|
|Score/Severity|Static: 1|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0003, _mitreAttackTechnique:T1136, _mitreAttackTechnique:T1136.003|
## Vendors and Products
- [Alibaba - ActionTrail](../products/79055042-52c8-4998-b201-bd2cd2dbca1f.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|action|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|user_username|


