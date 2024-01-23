# [Rules](README.md): AWS ECS Cluster Deleted

## Description
Monitors for execution of the API call 'DeleteCluster' which may indicate that an attacker is attempting to disrupt operations.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Impact|
|Apply Risk to Entities|device_hostname, device_ip, user_username, srcDevice_ip|
|Signal Name|AWS ECS Cluster Deleted|
|Summary Expression|{{action}} performed by user: {{user_username}}|
|Score/Severity|Static: 4|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0005, _mitreAttackTechnique:T1578, _mitreAttackTechnique:T1578.003|
## Vendors and Products
- [Amazon AWS - CloudTrail](../products/033624b0-218e-4dcb-b93f-0f1fb1806c56.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|listMatches|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|user_username|


