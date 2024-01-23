# [Rules](README.md): AWS EKS Secrets Created

## Description
Kubernetes secrets may be created for legitimate purposes, ensure that this secrets created is from an IAM account that is expected to manage Kubernetes workloads on EKS.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Credential Access|
|Apply Risk to Entities|srcDevice_ip|
|Signal Name|AWS EKS Secrets Created|
|Summary Expression|A Kubernetes secret was created within an AWS EKS cluster from {{srcDevice_ip}}|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0006, _mitreAttackTechnique:T1552.007|
## Vendors and Products
- [Amazon AWS - EKS](../products/234ec2b5-4142-4837-bc78-95da8a2db81a.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|action|
|Normalized Schema|cloud_provider|
|Normalized Schema|cloud_service|
|Direct from Record|fields["message.objectRef.resource"]|
|Normalized Schema|http_response_statusCode|
|Normalized Schema|srcDevice_ip|


