# [Rules](README.md): High risk file extension download without hostname and referrer

## Description
Although executable and dynamic-link libraries (.exe, .dll) are regularly downloaded from the Internet, benign ones are normally downloaded with the hostname and referrer fields populated. Thus, downloads from an IP address without referrer carry an elevated risk.

## Additional Details
|Detail|Value|
|----|----|
|Type|Match|
|Category|Persistence|
|Apply Risk to Entities|srcDevice_ip, user_username, device_hostname|
|Signal Name|High risk file extension download without hostname and referrer|
|Summary Expression|High risk file from URL: {{http_url}} with no hostname or referer present|
|Score/Severity|Static: 4|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0002, _mitreAttackTactic:TA0001, _mitreAttackTechnique:T1204, _mitreAttackTechnique:T1190, _mitreAttackTechnique:T1566, _mitreAttackTechnique:T1566.002, _mitreAttackTechnique:T1204.003, _mitreAttackTechnique:T1204.002, _mitreAttackTechnique:T1204.001|
## Vendors and Products
- [Bro - Bro](../products/37C866BF-72E1-470A-9072-EDB908F56951.md)
- [CheckPoint - SmartDefense](../products/2b82e665-bdde-474a-ae29-4f0f76598556.md)
- [CheckPoint - URL Filtering](../products/2a678bcd-898e-43cd-ab3f-91feb0602a18.md)
- [Cisco Systems - ASA](../products/be4f7473-fe69-4311-8859-3561900060bf.md)
- [Cisco Systems - Firepower](../products/da9e05a5-3fd3-46a7-a107-ae03c01e3f5a.md)
- [Cisco Systems - Meraki](../products/724c9add-8cd9-4013-b9e1-a907b96da426.md)
- [Forcepoint - Web Security](../products/e90edc67-68d4-4d67-82f6-4524f94b59bb.md)
- [Fortinet - Fortigate](../products/c57e2c85-4fc1-4fb7-8fa1-dbc5235231ad.md)
- [Juniper - SRX Series Firewall](../products/A17B3F3C-04F1-40C8-9497-3C499EB18A74.md)
- [Microsoft - Defender Advanced Hunting](../products/3382523e-2072-41bd-b50b-6b148957d0b0.md)
- [Netskope - Security Cloud](../products/B3582ED2-1A0C-452D-9802-97433D143486.md)
- [Palo Alto Networks - Next Generation Firewall](../products/46f5fa2c-1a62-4692-82ad-ed87800a0adb.md)
- [Palo Alto Networks - Prisma Cloud](../products/343b9323-d279-40d9-946f-809242e5cf98.md)
- [Sophos - UTM 9](../products/0fb003bc-8383-442f-8f3d-afcfbaefe617.md)
- [Zscaler - Nanolog Streaming Service](../products/6299d728-14f7-455e-85c5-ea8ec65a654a.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|device_hostname|
|Normalized Schema|dstDevice_ip_isInternal|
|Normalized Schema|http_hostname|
|Normalized Schema|http_referer|
|Normalized Schema|http_url_fqdn|
|Normalized Schema|http_url_path|
|Normalized Schema|http_url_rootDomain|
|Normalized Schema|listMatches|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|user_username|


