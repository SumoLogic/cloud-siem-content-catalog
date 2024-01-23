# [Rules](README.md): AWS CloudTrail - ScheduleKeyDeletion in KMS

## Description
Deleting cryptographic key material managed by KMS can be risky. The risk is that after key material is deleted, cypher text may remain that is now indecipherable. Because of this risk, AWS enforces a minimum 7 day waiting period. A key cannot be deleted, it must first be scheduled for deletion by the system. This signal indicates that a key has been scheduled or canceled for deletion. This signal in context of other signals around this entity may describe a hostile pattern of attack.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Execution|
|Apply Risk to Entities|device_hostname, device_ip, user_username, srcDevice_ip|
|Signal Name|AWS CloudTrail - ScheduleKeyDeletion in KMS|
|Summary Expression|{{action}} performed by user: {{user_username}}|
|Score/Severity|Static: 2|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0006, _mitreAttackTechnique:T1552, _mitreAttackTechnique:T1552.004, _mitreAttackTechnique:T1552.005|
## Vendors and Products
- [Amazon AWS - CloudTrail](../products/033624b0-218e-4dcb-b93f-0f1fb1806c56.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|user_username|


