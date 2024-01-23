# [Rules](README.md): Kubernetes AWS Suspicious kubectl Calls

## Description
Kubectl calls are not malicious by nature. However IP, user and user agent can reveal potential malicious activity, specially anonymous users suspicious IPs and sensitive objects such as configmaps or secrets.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Discovery|
|Apply Risk to Entities|device_ip, user_username|
|Signal Name|Kubernetes AWS Suspicious kubectl Calls|
|Summary Expression|Suspicious kubectl call from user: {{user_username}} and IP: {{device_ip}}|
|Score/Severity|Static: 1|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTechnique:T1526, _mitreAttackTactic:TA0007, _mitreAttackTactic:TA0002, _mitreAttackTechnique:T1106|
## Vendors and Products
- [Amazon AWS - CloudWatch](../products/b57c366d-e6a5-4e61-b950-5686a902bc24.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|device_ip|
|Normalized Schema|http_userAgent|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|user_username|


