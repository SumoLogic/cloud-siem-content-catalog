# [Rules](README.md): HTTP Response Error Spike to AWS EKS

## Description
HTTP web services provide response codes to client requests. The response code numbers in the 400s are used to indicate a client related error and response code numbers in the 500s represent server related errors. This rule looks for a AWS EKS cluster receiving a large frequency of web errors within a short period of time. It is unusual for a web client to cause this many errors in a short period of time. Common occurrences for this behavior is scanning/probing activity or scripted web clients which are now encountering errors due to a misconfiguration or recent change. This rule alerts when a host on the monitored network triggers the threshold.

## Additional Details
|Detail|Value|
|----|----|
|Type|Threshold|
|Category|Discovery|
|Apply Risk to Entities|srcDevice_ip|
|Signal Name|HTTP Response Error Spike to AWS EKS|
|Summary Expression|High number of HTTP response errors from an AWS EKS Cluster from {{srcDevice_ip}}|
|Threshold Count|700|
|Threshold Window|CUSTOM|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0007, _mitreAttackTactic:TA0011, _mitreAttackTactic:TA0043, _mitreAttackTechnique:T1595.001, _mitreAttackTechnique:T1190|
## Vendors and Products
- [Amazon AWS - EKS](../products/234ec2b5-4142-4837-bc78-95da8a2db81a.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|cloud_provider|
|Normalized Schema|cloud_service|
|Normalized Schema|http_response_statusCode|
|Normalized Schema|metadata_vendor|
|Normalized Schema|srcDevice_ip|


