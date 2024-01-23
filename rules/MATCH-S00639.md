# [Rules](README.md): Kubernetes Anonymous Request Authorized

## Description
Detect when an unauthenticated request user is permitted in Kubernetes.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Credential Access|
|Apply Risk to Entities|device_hostname, device_ip, user_username, dstDevice_ip|
|Signal Name|Kubernetes Anonymous Request Authorized|
|Summary Expression|Unauthentication user: {{user_username}} permitted|
|Score/Severity|Static: 2|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0006, _mitreAttackTactic:TA0001, _mitreAttackTechnique:T1078, _mitreAttackTechnique:T1078.004, _mitreAttackTechnique:T1552, _mitreAttackTechnique:T1552.007|
## Vendors and Products


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|dstDevice_ip|
|Normalized Schema|http_response_statusCode|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|user_username|


