# [Rules](README.md): Alibaba ActionTrail Network Access Control List Deleted

## Description
Enforcing network-access controls is one of the defensive mechanisms used by cloud administrators to restrict access to a cloud instance. After the attacker has gained control of the console by compromising an admin account, they can delete a network ACL and gain access to the instance from anywhere.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Unknown/Other|
|Apply Risk to Entities|srcDevice_ip, user_username|
|Signal Name|Alibaba ActionTrail Network Access Control List Deleted|
|Summary Expression|User: {{user_username}} from source IP: {{srcDevice_ip}} deleted a Network ACL|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0005, _mitreAttackTechnique:T1562, _mitreAttackTechnique:T1562.007|
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


