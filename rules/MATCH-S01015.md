# [Rules](README.md): Threat Intel - HTTP URL

## Description
This rule detects a URL indicator match from a threat intelligence feed

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Threat Intelligence|
|Apply Risk to Entities|device_hostname, srcDevice_hostname, device_ip, device_natIp, srcDevice_ip, srcDevice_natIp, device_mac, srcDevice_mac, user_username, dns_replyIp|
|Signal Name|Threat Intel - HTTP URL|
|Summary Expression|Threat Intel - HTTP URL detected for: {{http_url}}|
|Score/Severity|Static: 2|
|Enabled by Default|True|
|Prototype|False|
|Tags||
## Vendors and Products
- [CheckPoint - Firewall and VPN](../products/c3c1a4fc-10cc-4155-8a30-a3bb14fc9f31.md)
- [CheckPoint - URL Filtering](../products/2a678bcd-898e-43cd-ab3f-91feb0602a18.md)
- [Cisco Systems - Firepower](../products/da9e05a5-3fd3-46a7-a107-ae03c01e3f5a.md)
- [Cisco Systems - Meraki](../products/724c9add-8cd9-4013-b9e1-a907b96da426.md)
- [Cisco Systems - Umbrella](../products/5ba50e74-3c05-4ea8-aeaf-5efde588c60f.md)
- [Cloudflare - Logpush](../products/c2503fcc-ef30-4e40-bb32-0bf47151b140.md)
- [Extrahop - Reveal(x)](../products/78150d37-623d-471b-b7c9-fdefcadd21fa.md)
- [Forcepoint - Web Security](../products/e90edc67-68d4-4d67-82f6-4524f94b59bb.md)
- [Fortinet - Fortigate](../products/c57e2c85-4fc1-4fb7-8fa1-dbc5235231ad.md)
- [McAfee - Web Gateway](../products/003d35b3-3ba8-4e93-8776-e5810b4e243e.md)
- [Microsoft - Azure](../products/a1225af5-e778-4068-a9a2-47da93d1ff24.md)
- [Microsoft - Defender Advanced Hunting](../products/3382523e-2072-41bd-b50b-6b148957d0b0.md)
- [Microsoft - Graph Security API](../products/ef42eb74-7444-4fee-b231-b4eb1e7c9660.md)
- [Microsoft - Office 365](../products/d3ed003d-5ddd-4c7a-bea5-63eae6311833.md)
- [Netskope - Security Cloud](../products/B3582ED2-1A0C-452D-9802-97433D143486.md)
- [Palo Alto Networks - Next Generation Firewall](../products/46f5fa2c-1a62-4692-82ad-ed87800a0adb.md)
- [Proofpoint - Targeted Attack Protection](../products/de3d4b6b-36a3-4436-8bfc-0561ac95037e.md)
- [Squid - Squid Proxy](../products/af61d8a8-3eba-42fb-9f17-87443924f3f4.md)
- [Symantec - Web Security Service](../products/bf865cb5-0b26-4010-8b3c-5ae2d1f716d8.md)
- [Trend Micro - Apex Central](../products/F362EA03-9BBB-4701-B2DF-5460C4A289CF.md)
- [Zscaler - Firewall](../products/9e0641a7-22ce-4ac8-8113-ee48b368ac3d.md)
- [Zscaler - Nanolog Streaming Service](../products/6299d728-14f7-455e-85c5-ea8ec65a654a.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|OR|
|Normalized Schema|confidence|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|device_mac|
|Normalized Schema|device_natIp|
|Normalized Schema|dns_replyIp|
|Normalized Schema|listMatches|
|Normalized Schema|srcDevice_hostname|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|srcDevice_mac|
|Normalized Schema|srcDevice_natIp|
|Normalized Schema|type|
|Normalized Schema|user_username|


