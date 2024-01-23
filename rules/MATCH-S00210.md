# [Rules](README.md): AWS CloudTrail - SQS List Queues Event

## Description
This event sourced from AWS SQS occurs rarely.  It could indicate that an adversary is attempting to collect information for later attack.  When successful, the List Queues event returns all SQS queues that may be valid targets for further probing/attack.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Discovery|
|Apply Risk to Entities|device_hostname, device_ip, user_username, srcDevice_ip|
|Signal Name|AWS CloudTrail - SQS List Queues Event|
|Summary Expression|{{action}} performed by user: {{user_username}}|
|Score/Severity|Static: 2|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0007, _mitreAttackTechnique:T1526|
## Vendors and Products
- [Amazon AWS - CloudTrail](../products/033624b0-218e-4dcb-b93f-0f1fb1806c56.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|action|
|Normalized Schema|application|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|user_username|


