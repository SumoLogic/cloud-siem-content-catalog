# [Rules](README.md): HTTP CloudFlare Protocol Violation or Empty Response

## Description
Error code 520 is used as a catch-all status when the origin server returns something that is unexpected, not tolerated, or not interpreted. This can include protocol violations and empty responses.

## Additional Details
|Detail|Value|
|----|----|
|Type|Match|
|Category|Unknown/Other|
|Apply Risk to Entities|device_ip, srcDevice_ip, dstDevice_ip, device_hostname, srcDevice_hostname, dstDevice_hostname|
|Signal Name|HTTP CloudFlare Protocol Violation or Empty Response|
|Summary Expression|HTTP 502 Response from IP: {{srcDevice_ip}} to IP: {{dstDevice_ip}}|
|Score/Severity|Static: 1|
|Enabled by Default|False|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0001, _mitreAttackTechnique:T1190|
## Vendors and Products
- [Bro - Bro](../products/37C866BF-72E1-470A-9072-EDB908F56951.md)
- [Cisco Systems - Umbrella](../products/5ba50e74-3c05-4ea8-aeaf-5efde588c60f.md)
- [Cloudflare - Logpush](../products/c2503fcc-ef30-4e40-bb32-0bf47151b140.md)
- [McAfee - Web Gateway](../products/003d35b3-3ba8-4e93-8776-e5810b4e243e.md)
- [Sophos - UTM 9](../products/0fb003bc-8383-442f-8f3d-afcfbaefe617.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|dstDevice_hostname|
|Normalized Schema|dstDevice_ip|
|Normalized Schema|http_response_statusCode|
|Normalized Schema|srcDevice_hostname|
|Normalized Schema|srcDevice_ip|


