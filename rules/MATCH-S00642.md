# [Rules](README.md): Kubernetes Service Account Created in Kube Namespace

## Description
Detect when a user is creating a service account in one of the Kubernetes default namespaces. The only users creating service accounts in the kube-system namespace should be cluster administrators. Furthermore, it is best practice to not run any cluster critical infrastructure in the kube-system namespace. The kube-public namespace is intended for kubernetes objects which should be readable by unauthenticated users. Thus, a service account should likely not be created in the kube-public namespace.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Execution|
|Apply Risk to Entities|device_hostname, device_ip, user_username, dstDevice_ip|
|Signal Name|Kubernetes Service Account Created in Kube Namespace|
|Summary Expression|User: {{user_username}} created service account|
|Score/Severity|Static: 2|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0003, _mitreAttackTechnique:T1136, _mitreAttackTechnique:T1136.003, _mitreAttackTechnique:T1136.001, _mitreAttackTechnique:T1136.002|
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


