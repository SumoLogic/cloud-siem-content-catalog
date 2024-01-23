# [Rules](README.md): Alibaba ActionTrail Key Deleted or Disabled

## Description
Deleting cryptographic key material managed by KMS can be risky. The risk is that after key material is deleted, cypher text may remain that is now indecipherable. This signal indicates that a key has been scheduled or canceled for deletion. This signal in context of other signals around this entity may describe a hostile pattern of attack.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Unknown/Other|
|Apply Risk to Entities|user_username, srcDevice_ip|
|Signal Name|Alibaba ActionTrail Key Deleted or Disabled|
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
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|user_username|


