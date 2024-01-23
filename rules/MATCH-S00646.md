# [Rules](README.md): Kubernetes User Exec into a Pod

## Description
Detect when a user execs into a pod. A user should not need to exec into a pod. Execing into a pod allows a user to execute any process in container which is not already running. It is most common to execute the bash process to gain an interactive shell. If this is an attacker, they can access any data which the pod has permissions to, including secrets.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Execution|
|Apply Risk to Entities|device_hostname, device_ip, user_username, dstDevice_ip|
|Signal Name|Kubernetes User Exec into a Pod|
|Summary Expression|User: {{user_username}} exec into pod|
|Score/Severity|Static: 2|
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


