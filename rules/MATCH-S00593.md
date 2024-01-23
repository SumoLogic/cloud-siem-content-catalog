# [Rules](README.md): Alibaba ActionTrail ListQueues

## Description
This could indicate that an adversary is attempting to collect information for later attack.  When successful, the List Queues event returns all queues that may be valid targets for further probing/attack.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Unknown/Other|
|Apply Risk to Entities|srcDevice_ip, user_username|
|Signal Name|Alibaba ActionTrail ListQueues|
|Summary Expression|User: {{user_username}} from source IP: {{srcDevice_ip}} performed a List Keys action|
|Score/Severity|Static: 2|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0007, _mitreAttackTechnique:T1526|
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


