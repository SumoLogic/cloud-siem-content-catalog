# [Rules](README.md): New Cluster Admin Binding Role Created on AWS EKS

## Description
A cluster-admin role binding grants a resource superuser or administrative access to a Kubernetes cluster. Ensure this action is expected and performed by known Kubernetes administrators.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Defense Evasion|
|Apply Risk to Entities|srcDevice_ip|
|Signal Name|New Cluster Admin Binding Role Created on AWS EKS by {{srcDevice_ip}}|
|Summary Expression|New Cluster Admin Binding Role Created on AWS EKS by {{srcDevice_ip}}|
|Score/Severity|Static: 5|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0005, _mitreAttackTactic:TA0003, _mitreAttackTactic:TA0004, _mitreAttackTechnique:T1078.004|
## Vendors and Products
- [Amazon AWS - EKS](../products/234ec2b5-4142-4837-bc78-95da8a2db81a.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|action|
|Normalized Schema|cloud_provider|
|Normalized Schema|cloud_service|
|Normalized Schema|decision"]|
|Direct from Record|fields["message.responseObject.roleRef.name"]|
|Normalized Schema|srcDevice_ip|


