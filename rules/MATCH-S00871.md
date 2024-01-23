# [Rules](README.md): AWS EKS Pod Shared Object Modification or Creation

## Description
A Kubernetes pod was either created, updated or patched with a shared process namespace.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Privilege Escalation|
|Apply Risk to Entities|srcDevice_ip|
|Signal Name|AWS EKS Pod Shared Object Modification or Creation from {{srcDevice_ip}}|
|Summary Expression|A Kubernetes pod was either created, updated or patched with a shared process namespace.|
|Score/Severity|Dynamic: 3 or 5|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0004, _mitreAttackTechnique:T1611|
## Vendors and Products
- [Amazon AWS - EKS](../products/234ec2b5-4142-4837-bc78-95da8a2db81a.md)


## Dynamic Signal Score/Severity Translation

The default score of `3` is used as a catch all if none of the translations are met.

|Schema Field|Field Value|Score/Severity|
|------------|-----------|--------------|
|http_response_statusCode|201|5|
|http_response_statusCode|400|3|
|http_response_statusCode|300|0|
## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|action|
|Normalized Schema|cloud_provider|
|Normalized Schema|cloud_service|
|Direct from Record|fields["message.requestObject.spec.shareProcessNamespace"]|
|Normalized Schema|http_response_statusCode|
|Normalized Schema|srcDevice_ip|


