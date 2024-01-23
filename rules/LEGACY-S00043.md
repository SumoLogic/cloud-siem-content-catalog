# [Rules](README.md): HTTP Request with Single Header

## Description
HTTP requests typically have multiple headers. It is odd in some cases if the event only contains a single header. This produces a low severity signal when an HTTP event is observed containing only one header in the request.

## Additional Details
|Detail|Value|
|----|----|
|Type|Match|
|Category|Initial Access|
|Apply Risk to Entities|srcDevice_ip|
|Signal Name|HTTP Request with Single Header|
|Summary Expression|HTTP request from IP: {{srcDevice_ip}} to URL: {{http_url}}|
|Score/Severity|Static: 1|
|Enabled by Default|False|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0001, _mitreAttackTactic:TA0011, _mitreAttackTechnique:T1071, _mitreAttackTechnique:T1071.001|
## Vendors and Products
- [Bro - Bro](../products/37C866BF-72E1-470A-9072-EDB908F56951.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|bro_http_request_headers|
|Normalized Schema|dstDevice_ip_isInternal|
|Normalized Schema|http_response_statusCode|
|Normalized Schema|listMatches|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|srcDevice_ip_isInternal|


