# [Rules](README.md): First Seen AWS EKS Secrets Enumeration from IP Address

## Description
Adversaries may enumerate various Kubernetes secrets in order to escalate privileges or to look for persistence avenues.

## Additional Details
|Detail|Value|
|----|----|
|Type|First Seen|
|Category|Discovery|
|Apply Risk to Entities|srcDevice_ip|
|Signal Name|First Seen AWS EKS Secrets Enumeration from {{srcDevice_ip}}|
|Summary Expression|{{srcDevice_ip}} has enumerated secrets on an AWS EKS cluster for the first time since the baseline period.|
|Retention Window|7776000000|
|Baseline Window|1814400000|
|Baseline Type|GLOBAL|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0007, _mitreAttackTechnique:T1613|
## Vendors and Products
- [Amazon AWS - EKS](../products/234ec2b5-4142-4837-bc78-95da8a2db81a.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|action|
|Normalized Schema|cloud_provider|
|Normalized Schema|cloud_service|
|Direct from Record|fields["message.objectRef.resource"]|
|Direct from Record|fields["message.stage"]|
|Normalized Schema|http_response_statusCode|
|Normalized Schema|http_userAgent|
|Normalized Schema|matches|
|Normalized Schema|srcDevice_ip|


