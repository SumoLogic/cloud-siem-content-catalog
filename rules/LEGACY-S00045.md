# [Rules](README.md): HTTP request for single character file name

## Description
Many threats are served from websites using lazy single character based filenames like 1.exe, etc. These nondescript file names are rare with most legitimate content. This rule looks for requests to retrieve high risk file extensions from such paths.

## Additional Details
|Detail|Value|
|----|----|
|Type|Match|
|Category|Execution|
|Apply Risk to Entities|srcDevice_ip|
|Signal Name|HTTP request for single character file name|
|Summary Expression|HTTP request from IP: {{srcDevice_ip}} to URL: {{http_url}}|
|Score/Severity|Static: 4|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0002, _mitreAttackTactic:TA0011, _mitreAttackTechnique:T1071, _mitreAttackTechnique:T1071.001|
## Vendors and Products
- [Amazon AWS - Web Application Firewall (WAF)](../products/072b85a2-1765-45c2-911d-b0509880326e.md)
- [Bro - Bro](../products/37C866BF-72E1-470A-9072-EDB908F56951.md)
- [Cisco Systems - Meraki](../products/724c9add-8cd9-4013-b9e1-a907b96da426.md)
- [Cloudflare - Logpush](../products/c2503fcc-ef30-4e40-bb32-0bf47151b140.md)
- [Fortinet - Fortigate](../products/c57e2c85-4fc1-4fb7-8fa1-dbc5235231ad.md)
- [Netskope - Security Cloud](../products/B3582ED2-1A0C-452D-9802-97433D143486.md)
- [Palo Alto Networks - Next Generation Firewall](../products/46f5fa2c-1a62-4692-82ad-ed87800a0adb.md)
- [Sophos - UTM 9](../products/0fb003bc-8383-442f-8f3d-afcfbaefe617.md)
- [Zscaler - Firewall](../products/9e0641a7-22ce-4ac8-8113-ee48b368ac3d.md)
- [Zscaler - Nanolog Streaming Service](../products/6299d728-14f7-455e-85c5-ea8ec65a654a.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|dstDevice_ip_isInternal|
|Normalized Schema|http_url_path|
|Normalized Schema|listMatches|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|srcDevice_ip_isInternal|


