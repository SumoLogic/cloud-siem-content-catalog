# [Rules](README.md): Threat Intel - Inbound Traffic from Threat Feed IP (High Confidence)

## Description
This rule detects traffic to IP address with a high confidence rating from a threat intelligence feed.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Threat Intelligence|
|Apply Risk to Entities|srcDevice_ip, dstDevice_ip, device_ip, srcDevice_ip, srcDevice_hostname, srcDevice_hostname, dstDevice_hostname, device_hostname, user_username|
|Signal Name|Threat Intel - Inbound Traffic From a High Confidence Threat IP|
|Summary Expression|Successful inbound network traffic from Threat IP address {{srcDevice_ip}}}|
|Score/Severity|Static: 0|
|Enabled by Default|True|
|Prototype|False|
|Tags||
## Vendors and Products
- [Amazon AWS - AWS S3 Server Access Logs](../products/41f70c6e-18a9-462c-a04d-4edc7baead7a.md)
- [Amazon AWS - VpcFlowLogs](../products/021d1ded-1c82-4663-bf5d-d6ed5170efa3.md)
- [Amazon AWS - Web Application Firewall (WAF)](../products/072b85a2-1765-45c2-911d-b0509880326e.md)
- [CheckPoint - Firewall and VPN](../products/c3c1a4fc-10cc-4155-8a30-a3bb14fc9f31.md)
- [CheckPoint - SmartDefense](../products/2b82e665-bdde-474a-ae29-4f0f76598556.md)
- [CheckPoint - URL Filtering](../products/2a678bcd-898e-43cd-ab3f-91feb0602a18.md)
- [Cisco Systems - ASA](../products/be4f7473-fe69-4311-8859-3561900060bf.md)
- [Cisco Systems - Meraki](../products/724c9add-8cd9-4013-b9e1-a907b96da426.md)
- [Cisco Systems - Umbrella](../products/5ba50e74-3c05-4ea8-aeaf-5efde588c60f.md)
- [Citrix - ADC](../products/d3606245-76d3-4173-a2fe-832c0e71b0f9.md)
- [Fortinet - Fortigate](../products/c57e2c85-4fc1-4fb7-8fa1-dbc5235231ad.md)
- [Google - BigQuery](../products/a67d97fe-6e68-4cfb-9500-cfc5492da565.md)
- [Google - Google Cloud Platform](../products/dcc85cfc-a698-4d09-87de-f2c723f3ad07.md)
- [Juniper - SRX Series Firewall](../products/A17B3F3C-04F1-40C8-9497-3C499EB18A74.md)
- [Linux - Systemd Journal](../products/5be5af82-c248-4c4c-a485-0571025f242c.md)
- [Microsoft - Azure](../products/a1225af5-e778-4068-a9a2-47da93d1ff24.md)
- [Microsoft - O365 Exchange Message Trace](../products/183c5127-6594-4d45-9bab-ce5f2df9e38b.md)
- [Microsoft - Office 365](../products/d3ed003d-5ddd-4c7a-bea5-63eae6311833.md)
- [Okta - Single Sign-On](../products/51278354-d6b5-4c8e-a8fd-8197df334e67.md)
- [Palo Alto Networks - Next Generation Firewall](../products/46f5fa2c-1a62-4692-82ad-ed87800a0adb.md)
- [Proofpoint - Targeted Attack Protection](../products/de3d4b6b-36a3-4436-8bfc-0561ac95037e.md)
- [WatchGuard - Fireware](../products/14aa46d3-0710-44b6-9ce3-0a6b8f36b076.md)
- [Zscaler - Nanolog Streaming Service](../products/6299d728-14f7-455e-85c5-ea8ec65a654a.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|OR|
|Normalized Schema|confidence|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|dstDevice_hostname|
|Normalized Schema|dstDevice_ip|
|Normalized Schema|objectType|
|Normalized Schema|srcDevice_hostname|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|srcDevice_ip_isInternal|
|Normalized Schema|success|
|Normalized Schema|type|
|Normalized Schema|user_username|


