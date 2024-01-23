# [Rules](README.md): Kubernetes User Attached to a Pod

## Description
Detect when a user attaches to a pod. A user should not need to attach to a pod. Attaching to a pod allows a user to attach to any process in a running container which may give an attacker access to sensitive data.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Execution|
|Apply Risk to Entities|device_hostname, device_ip, user_username, dstDevice_ip|
|Signal Name|Kubernetes User Attached to a Pod|
|Summary Expression|User: {{user_username}} attached themselves to a pod.|
|Score/Severity|Static: 1|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0006, _mitreAttackTechnique:T1552, _mitreAttackTechnique:T1552.007|
## Vendors and Products


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|changeType|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|dstDevice_ip|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|resource|
|Normalized Schema|user_username|


