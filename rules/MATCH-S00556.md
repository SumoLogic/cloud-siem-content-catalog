# [Rules](README.md): Outbound Data Transfer Protocol Over Non-standard Port

## Description
This rule detects commonly used data transfer protocols being used over non-standard ports, which could indicate an attempt to obfuscate exfiltration or command and control activity.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Exfiltration|
|Apply Risk to Entities|srcDevice_ip, srcDevice_hostname|
|Signal Name|Outbound Data Transfer Protocol Over Non-standard Port|
|Summary Expression|Source IP {{srcDevice_ip}} communicated with {{dstDevice_ip}} using {{application}} over non-standard port {{dstPort}}.|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0010, _mitreAttackTactic:TA0011, _mitreAttackTechnique:T1571|
## Vendors and Products
- [Cato Networks - Cato Networks](../products/168afd8d-2893-4c74-95b1-a975d576ea56.md)
- [Cisco Systems - Firepower](../products/da9e05a5-3fd3-46a7-a107-ae03c01e3f5a.md)
- [Fortinet - Fortigate](../products/c57e2c85-4fc1-4fb7-8fa1-dbc5235231ad.md)
- [Juniper - SRX Series Firewall](../products/A17B3F3C-04F1-40C8-9497-3C499EB18A74.md)
- [McAfee - Network Security](../products/1ac6a4c6-c3b6-412b-bd34-bc9f0dd6abdc.md)
- [Palo Alto Networks - Cortex XDR](../products/146522A1-DC9A-40A5-A909-2EB3B665B1D1.md)
- [Palo Alto Networks - Next Generation Firewall](../products/46f5fa2c-1a62-4692-82ad-ed87800a0adb.md)
- [Palo Alto Networks - Prisma Cloud](../products/343b9323-d279-40d9-946f-809242e5cf98.md)
- [SonicWall - Firewall](../products/951a004d-54bf-441d-98e1-fcc6a032f475.md)
- [Zscaler - Firewall](../products/9e0641a7-22ce-4ac8-8113-ee48b368ac3d.md)
- [Zscaler - Nanolog Streaming Service](../products/6299d728-14f7-455e-85c5-ea8ec65a654a.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|dstDevice_ip_isInternal|
|Normalized Schema|dstPort|
|Normalized Schema|srcDevice_hostname|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|srcDevice_ip_isInternal|


