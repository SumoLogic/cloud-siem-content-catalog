# [Rules](README.md): Kubernetes Service Created with NodePort

## Description
Detect when a service’s port is attached to the node’s IP. Exposing the service’s port to the the node’s IP allows other hosts on the network namespace to access this service.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Execution|
|Apply Risk to Entities|device_hostname, device_ip, user_username, dstDevice_ip|
|Signal Name|Kubernetes Service Created with NodePort|
|Summary Expression|User: {{user_username}} created service|
|Score/Severity|Static: 2|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0006, _mitreAttackTechnique:T1552, _mitreAttackTechnique:T1552.007|
## Vendors and Products


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|dstDevice_ip|
|Direct from Record|fields['message.requestObject.spec.type']|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|resource|
|Normalized Schema|user_username|


