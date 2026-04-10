# [Rules](README.md): HTTP Request to Domain in Non-Standard TLD

## Description
HTTP request to a domain that is not under an ICANN-standard TLD. These TLDs are provided by alternate DNS root servers such as OpenNIC. Their use on corporate networks is fundamentally suspicious and potentially a sign of abuse by threat actors.

## Additional Details
|Detail|Value|
|----|----|
|Type|Match|
|Category|Command and Control|
|Apply Risk to Entities|srcDevice_ip|
|Signal Name|HTTP Request to Domain in Non-Standard TLD|
|Summary Expression|HTTP request from IP: {{srcDevice_ip}} to URL: {{http_url}}|
|Score/Severity|Static: 6|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0011, _mitreAttackTechnique:T1071, _mitreAttackTechnique:T1071.001|
## Vendors and Products
- [Akamai - SIEM](../products/9a28f2af-5526-414d-973b-c3fc7984b8a1.md)
- [Amazon AWS - Elastic Load Balancer](../products/59a3cd41-b6d2-4ab7-a0ff-6d5abd14ac43.md)
- [Bro - Bro](../products/37C866BF-72E1-470A-9072-EDB908F56951.md)
- [Cisco Systems - ASA](../products/be4f7473-fe69-4311-8859-3561900060bf.md)
- [Cisco Systems - Firepower](../products/da9e05a5-3fd3-46a7-a107-ae03c01e3f5a.md)
- [Cisco Systems - Meraki](../products/724c9add-8cd9-4013-b9e1-a907b96da426.md)
- [Cisco Systems - Umbrella](../products/5ba50e74-3c05-4ea8-aeaf-5efde588c60f.md)
- [Cloudflare - Logpush](../products/c2503fcc-ef30-4e40-bb32-0bf47151b140.md)
- [Fortinet - Fortigate](../products/c57e2c85-4fc1-4fb7-8fa1-dbc5235231ad.md)
- [Netskope - Security Cloud](../products/B3582ED2-1A0C-452D-9802-97433D143486.md)
- [Nginx - Nginx](../products/1ce88b4b-d90d-4d50-9a89-3abe83e8d5f8.md)
- [Palo Alto Networks - Next Generation Firewall](../products/46f5fa2c-1a62-4692-82ad-ed87800a0adb.md)
- [Trend Micro - Apex Central](../products/F362EA03-9BBB-4701-B2DF-5460C4A289CF.md)
- [Zscaler - Nanolog Streaming Service](../products/6299d728-14f7-455e-85c5-ea8ec65a654a.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|http_url_tld|
|Normalized Schema|srcDevice_ip|


