# [Rules](README.md): VBS file downloaded from Internet

## Description
Although Visual Basic scripts (.vbs) are sometimes regularly downloaded from the Internet, they are often part of malware establishment.  They carry an elevated risk.

## Additional Details
|Detail|Value|
|----|----|
|Type|Match|
|Category|Execution|
|Apply Risk to Entities|device_hostname, device_ip, srcDevice_hostname, srcDevice_ip, user_username|
|Signal Name|VBS file downloaded from Internet|
|Summary Expression|User: {{user_username}} download VBS file on IP: {{srcDevice_ip}} from URL: {{http_url}}|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0002, _mitreAttackTechnique:T1204, _mitreAttackTechnique:T1204.002, _mitreAttackTechnique:T1059, _mitreAttackTechnique:T1059.005|
## Vendors and Products
- [Amazon AWS - Web Application Firewall (WAF)](../products/072b85a2-1765-45c2-911d-b0509880326e.md)
- [Bro - Bro](../products/37C866BF-72E1-470A-9072-EDB908F56951.md)
- [CheckPoint - URL Filtering](../products/2a678bcd-898e-43cd-ab3f-91feb0602a18.md)
- [Cisco Systems - ASA](../products/be4f7473-fe69-4311-8859-3561900060bf.md)
- [Cisco Systems - Meraki](../products/724c9add-8cd9-4013-b9e1-a907b96da426.md)
- [Cloudflare - Logpush](../products/c2503fcc-ef30-4e40-bb32-0bf47151b140.md)
- [Forcepoint - Web Security](../products/e90edc67-68d4-4d67-82f6-4524f94b59bb.md)
- [Fortinet - Fortigate](../products/c57e2c85-4fc1-4fb7-8fa1-dbc5235231ad.md)
- [McAfee - Web Gateway](../products/003d35b3-3ba8-4e93-8776-e5810b4e243e.md)
- [Netskope - Security Cloud](../products/B3582ED2-1A0C-452D-9802-97433D143486.md)
- [Palo Alto Networks - Next Generation Firewall](../products/46f5fa2c-1a62-4692-82ad-ed87800a0adb.md)
- [Sophos - UTM 9](../products/0fb003bc-8383-442f-8f3d-afcfbaefe617.md)
- [Zscaler - Firewall](../products/9e0641a7-22ce-4ac8-8113-ee48b368ac3d.md)
- [Zscaler - Nanolog Streaming Service](../products/6299d728-14f7-455e-85c5-ea8ec65a654a.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|dstDevice_ip_isInternal|
|Normalized Schema|http_url|
|Normalized Schema|http_url_alexaRank|
|Normalized Schema|listMatches|
|Normalized Schema|srcDevice_hostname|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|user_username|


