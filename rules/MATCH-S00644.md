# [Rules](README.md): New Kubernetes Namespace Created

## Description
Detect when a user is creating a Kubernetes namespace.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Execution|
|Apply Risk to Entities|device_hostname, device_ip, user_username, dstDevice_ip|
|Signal Name|New Kubernetes Namespace Created|
|Summary Expression|Action: {{action}} performed by user: {{user_username}} from IP: {{srcDevice_ip}}|
|Score/Severity|Static: 1|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0002, _mitreAttackTechnique:T1204, _mitreAttackTechnique:T1609, _mitreAttackTechnique:T1610, _mitreAttackTechnique:T1204.003|
## Vendors and Products


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|dstDevice_ip|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|resource|
|Normalized Schema|user_username|


