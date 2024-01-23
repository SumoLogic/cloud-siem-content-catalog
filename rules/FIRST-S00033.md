# [Rules](README.md): First Seen Terminal-Attached Pod Deployed to EKS

## Description
A pod was deployed with an attached terminal (stdin=true,stdout=true,tty=true) for the first time since the baseline period.

## Additional Details
|Detail|Value|
|----|----|
|Type|First Seen|
|Category|Execution|
|Apply Risk to Entities|srcDevice_ip|
|Signal Name|First seen terminal-attached pod deployed on EKS from {{srcDevice_ip}}|
|Summary Expression|Upon gaining access to a Kubernetes cluster, attackers may want to deploy a container with a terminal attached in order to be able to communicate with other Kubernetes resources within the cluster. Ensure this activity matches normal Kubernetes administrative practices within the cluster.|
|Retention Window|7776000000|
|Baseline Window|1814400000|
|Baseline Type|PER_ENTITY|
|Score/Severity|Static: 2|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0002, _mitreAttackTechnique:T1610|
## Vendors and Products
- [Amazon AWS - EKS](../products/234ec2b5-4142-4837-bc78-95da8a2db81a.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|action|
|Normalized Schema|cloud_provider|
|Normalized Schema|cloud_service|
|Normalized Schema|srcDevice_ip|


