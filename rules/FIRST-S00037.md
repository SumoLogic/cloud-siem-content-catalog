# [Rules](README.md): First Seen AWS EKS Admission Controller Created by IP Address

## Description
First Seen Admission Controllers (Submit a new MutatingWebhookConfiguration or ValidatingWebhookConfiguration object via the Kubernetes API, or update an existing one.)

## Additional Details
|Detail|Value|
|----|----|
|Type|First Seen|
|Category|Defense Evasion|
|Apply Risk to Entities|srcDevice_ip|
|Signal Name|First Seen AWS EKS Admission Controller Created by {{srcDevice_ip}}|
|Summary Expression|An AWS EKS admission controller was created by an IP address: {{srcDevice_ip}} not seen since the baseline period.|
|Retention Window|7776000000|
|Baseline Window|1814400000|
|Baseline Type|GLOBAL|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTechnique:T1550, _mitreAttackTactic:TA0005, _mitreAttackTactic:TA0008|
## Vendors and Products
- [Amazon AWS - EKS](../products/234ec2b5-4142-4837-bc78-95da8a2db81a.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|action|
|Normalized Schema|cloud_provider|
|Normalized Schema|cloud_service|
|Direct from Record|fields["message.requestObject.kind"]|
|Normalized Schema|http_response_statusCode|
|Normalized Schema|srcDevice_ip|


