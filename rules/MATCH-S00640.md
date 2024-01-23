# [Rules](README.md): Kubernetes Pod Created in Kube Namespace

## Description
Detect when a user is creating a pod in one of the Kubernetes default namespaces. The only users creating pods in the kube-system namespace should be cluster administrators. Furthermore, it is best practice to not run any cluster critical infrastructure in the kube-system namespace. The kube-public namespace is intended for Kubernetes objects which should be readable by unauthenticated users. Thus, a pod should likely not be created in the kube-public namespace.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Execution|
|Apply Risk to Entities|device_hostname, device_ip, user_username, dstDevice_ip|
|Signal Name|Kubernetes Pod Created in Kube Namespace|
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
|Normalized Schema|device_k8s_namespace|
|Normalized Schema|dstDevice_ip|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|resource|
|Normalized Schema|user_username|


