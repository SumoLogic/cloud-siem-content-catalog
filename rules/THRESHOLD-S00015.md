# [Rules](README.md): HTTP Response Error Spike - External

## Description
HTTP web services provide response codes to client requests. The response code numbers in the 400s are used to indicate a client related error and response code numbers in the 500s represent server related errors. This rule looks for a web client receiving a large frequency of web errors within a short period of time. It is unusual for a web client to cause this many errors in a short period of time. Common occurrences for this behavior is scanning/probing activity or scripted web clients which are now encountering errors due to a misconfiguration or recent change. This rule alerts when a host external to the monitored network triggers the threshold.

## Additional Details
|Detail|Value|
|----|----|
|Type|Threshold|
|Category|Discovery|
|Apply Risk to Entities|device_ip, srcDevice_ip, dstDevice_ip, device_hostname, srcDevice_hostname, dstDevice_hostname|
|Signal Name|HTTP Response Error Spike - External|
|Summary Expression|High number of external HTTP response errors from IP: {{srcDevice_ip}} to {{dstDevice_ip}}|
|Threshold Count|350|
|Threshold Window|5m|
|Score/Severity|Static: 2|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0007, _mitreAttackTactic:TA0011, _mitreAttackTactic:TA0043, _mitreAttackTechnique:T1595, _mitreAttackTechnique:T1190, _mitreAttackTechnique:T1595.001, _mitreAttackTechnique:T1595.002, _mitreAttackTactic:TA0009, _mitreAttackTechnique:T1213, _mitreAttackTechnique:T1213.001|
## Vendors and Products
- [Amazon AWS - Application Load Balancer](../products/5bb9e0b3-8d57-4b10-8952-0b6ffe91b599.md)
- [Barracuda - Web Application Firewall](../products/798f8da8-c85b-4e9a-b2f1-eae0b07532fb.md)
- [Bro - Bro](../products/37C866BF-72E1-470A-9072-EDB908F56951.md)
- [Cloudflare - Logpush](../products/c2503fcc-ef30-4e40-bb32-0bf47151b140.md)
- [Microsoft - Azure](../products/a1225af5-e778-4068-a9a2-47da93d1ff24.md)
- [Microsoft - IIS](../products/fca8785d-4823-4442-86b2-8acbaa176da4.md)
- [Zscaler - Nanolog Streaming Service](../products/6299d728-14f7-455e-85c5-ea8ec65a654a.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|dstDevice_hostname|
|Normalized Schema|dstDevice_ip|
|Normalized Schema|dstDevice_ip_isInternal|
|Normalized Schema|http_response_statusCode|
|Normalized Schema|srcDevice_hostname|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|srcDevice_ip_isInternal|


