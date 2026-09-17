# [Rules](README.md): GCP Audit Key Deleted or Disabled

## Description
Deleting cryptographic key material managed by KMS can be risky. The risk is that after key material is deleted, cypher text may remain that is now indecipherable. This signal indicates that a key has been scheduled or canceled for deletion. This signal in context of other signals around this entity may describe a hostile pattern of attack.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Persistence|
|Apply Risk to Entities|user_username, srcDevice_ip|
|Signal Name|GCP Audit Key Deleted or Disabled|
|Summary Expression|User: {{user_username}} performed action: {{action}}|
|Score/Severity|Static: 6|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0003, _mitreAttackTechnique:T1485, _mitreAttackTactic:TA0006, _mitreAttackTechnique:T1552, _mitreAttackTechnique:T1552.004, _mitreAttackTechnique:T1552.005|
## Vendors and Products
- [Google - Google Cloud Platform](../products/dcc85cfc-a698-4d09-87de-f2c723f3ad07.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|action|
|Normalized Schema|application|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|user_username|


