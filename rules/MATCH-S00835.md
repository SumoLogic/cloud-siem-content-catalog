# [Rules](README.md): Possible Dynamic URL Domain

## Description
This rule looks for URL/refferer domains which appear to be associated with a dynamic DNS service.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Command and Control|
|Apply Risk to Entities|device_hostname, device_ip, srcDevice_hostname, srcDevice_ip, user_username|
|Signal Name|Possible Dynamic URL Domain|
|Summary Expression|Possible dynamic DNS domain for URL: {{http_url_fqdn}}|
|Score/Severity|Static: 1|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0011, _mitreAttackTechnique:T1568, _mitreAttackTechnique:T1568.001, _mitreAttackTechnique:T1568.002, _mitreAttackTechnique:T1568.003|
## Vendors and Products
- [Amazon AWS - Application Load Balancer](../products/5bb9e0b3-8d57-4b10-8952-0b6ffe91b599.md)
- [Amazon AWS - CloudFront](../products/44f07c08-c2ad-4a95-a058-1d0737ff90db.md)
- [Amazon AWS - Web Application Firewall (WAF)](../products/072b85a2-1765-45c2-911d-b0509880326e.md)
- [Bro - Bro](../products/37C866BF-72E1-470A-9072-EDB908F56951.md)
- [CheckPoint - URL Filtering](../products/2a678bcd-898e-43cd-ab3f-91feb0602a18.md)
- [Cisco Systems - Firepower](../products/da9e05a5-3fd3-46a7-a107-ae03c01e3f5a.md)
- [Cisco Systems - Ironport](../products/c07b5749-deda-4c7e-8e78-4a5dec1fcf4d.md)
- [Cisco Systems - Meraki](../products/724c9add-8cd9-4013-b9e1-a907b96da426.md)
- [Cisco Systems - Umbrella](../products/5ba50e74-3c05-4ea8-aeaf-5efde588c60f.md)
- [Cloudflare - Logpush](../products/c2503fcc-ef30-4e40-bb32-0bf47151b140.md)
- [Dell - Firewall](../products/b1639f7f-4c11-4d29-ab69-368cf0e05e25.md)
- [Forcepoint - Web Security](../products/e90edc67-68d4-4d67-82f6-4524f94b59bb.md)
- [Fortinet - Fortigate](../products/c57e2c85-4fc1-4fb7-8fa1-dbc5235231ad.md)
- [Juniper - SRX Series Firewall](../products/A17B3F3C-04F1-40C8-9497-3C499EB18A74.md)
- [McAfee - Web Gateway](../products/003d35b3-3ba8-4e93-8776-e5810b4e243e.md)
- [Microsoft - Azure](../products/a1225af5-e778-4068-a9a2-47da93d1ff24.md)
- [Microsoft - Defender Advanced Hunting](../products/3382523e-2072-41bd-b50b-6b148957d0b0.md)
- [Microsoft - IIS](../products/fca8785d-4823-4442-86b2-8acbaa176da4.md)
- [Netskope - Security Cloud](../products/B3582ED2-1A0C-452D-9802-97433D143486.md)
- [Palo Alto Networks - Next Generation Firewall](../products/46f5fa2c-1a62-4692-82ad-ed87800a0adb.md)
- [Proofpoint - Targeted Attack Protection](../products/de3d4b6b-36a3-4436-8bfc-0561ac95037e.md)
- [Sophos - UTM 9](../products/0fb003bc-8383-442f-8f3d-afcfbaefe617.md)
- [Squid - Squid Proxy](../products/af61d8a8-3eba-42fb-9f17-87443924f3f4.md)
- [Symantec - Proxy Secure Gateway](../products/991a55cf-8c5a-49ba-ae72-6f64a002bacf.md)
- [Symantec - Web Security Service](../products/bf865cb5-0b26-4010-8b3c-5ae2d1f716d8.md)
- [Trend Micro - Apex Central](../products/F362EA03-9BBB-4701-B2DF-5460C4A289CF.md)
- [Zscaler - Firewall](../products/9e0641a7-22ce-4ac8-8113-ee48b368ac3d.md)
- [Zscaler - Nanolog Streaming Service](../products/6299d728-14f7-455e-85c5-ea8ec65a654a.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|http_referer_alexaRank|
|Normalized Schema|http_referer_possibleDynDns|
|Normalized Schema|http_url_alexaRank|
|Normalized Schema|http_url_possibleDynDns|
|Normalized Schema|srcDevice_hostname|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|user_username|


