# [Rules](README.md): GCP Audit ListQueues

## Description
This could indicate that an adversary is attempting to collect information for later attack. When successful, the List Queues event returns all queues that may be valid targets for further probing/attack.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Discovery|
|Apply Risk to Entities|user_username, srcDevice_ip|
|Signal Name|GCP Audit ListQueues|
|Summary Expression|User: {{user_username}} performed action: {{action}}|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0043, _mitreAttackTactic:TA0007, _mitreAttackTechnique:T1526|
## Vendors and Products
- [Google - Google Cloud Platform](../products/dcc85cfc-a698-4d09-87de-f2c723f3ad07.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|action|
|Normalized Schema|description|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|user_username|


