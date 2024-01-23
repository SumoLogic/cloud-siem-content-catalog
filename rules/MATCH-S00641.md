# [Rules](README.md): Kubernetes Pod Created with hostNetwork

## Description
Detect when a pod is attached to the host network. Attaching the hostNetwork permits a pod to access the node’s network adapter allowing a pod to listen to all network traffic for all pods on the node and communicate with other pods on the network namespace.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Execution|
|Apply Risk to Entities|device_hostname, device_ip, user_username, dstDevice_ip|
|Signal Name|Kubernetes Pod Created with hostNetwork|
|Summary Expression|User: {{user_username}} created pod|
|Score/Severity|Static: 1|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0002, _mitreAttackTechnique:T1609, _mitreAttackTechnique:T1610, _mitreAttackTechnique:T1204, _mitreAttackTechnique:T1204.003|
## Vendors and Products


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|dstDevice_ip|
|Direct from Record|fields['message.requestObject.spec.hostNetwork']|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|resource|
|Normalized Schema|user_username|


