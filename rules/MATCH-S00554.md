# [Rules](README.md): Outbound IRC Traffic

## Description
This rule detects outbound traffic over IRC, which could indicate a compromised host being used for command and control or exfiltration operations.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Command and Control|
|Apply Risk to Entities|srcDevice_hostname, srcDevice_ip, user_username|
|Signal Name|Outbound IRC Traffic|
|Summary Expression|Outbound IRC traffic from IP: {{srcDevice_ip}} to IP: {{dstDevice_ip}}|
|Score/Severity|Dynamic: 1 or 3|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0011, _mitreAttackTechnique:T1071, _mitreAttackTechnique:T1071.001|
## Vendors and Products
- [Amazon AWS - Network Firewall](../products/3a82061c-2ca3-4289-9c9b-78756001aa38.md)
- [Amazon AWS - VPC Transit Gateways Flow Logs](../products/0e3d5c19-0a50-4ecf-b6f9-b1410d5dbb63.md)
- [Amazon AWS - VpcFlowLogs](../products/021d1ded-1c82-4663-bf5d-d6ed5170efa3.md)
- [Amazon AWS - Web Application Firewall (WAF)](../products/072b85a2-1765-45c2-911d-b0509880326e.md)
- [Barracuda - CloudGen Firewall](../products/34dd9c1e-ceec-4cba-8f5d-4776f680d785.md)
- [Barracuda - Web Application Firewall](../products/798f8da8-c85b-4e9a-b2f1-eae0b07532fb.md)
- [Bro - Bro](../products/37C866BF-72E1-470A-9072-EDB908F56951.md)
- [CheckPoint - Application Control](../products/1624169f-36c4-4309-8400-1409a171d00b.md)
- [CheckPoint - Firewall and VPN](../products/c3c1a4fc-10cc-4155-8a30-a3bb14fc9f31.md)
- [CheckPoint - SmartDefense](../products/2b82e665-bdde-474a-ae29-4f0f76598556.md)
- [CheckPoint - URL Filtering](../products/2a678bcd-898e-43cd-ab3f-91feb0602a18.md)
- [Cisco Systems - ASA](../products/be4f7473-fe69-4311-8859-3561900060bf.md)
- [Cisco Systems - Firepower](../products/da9e05a5-3fd3-46a7-a107-ae03c01e3f5a.md)
- [Cisco Systems - Meraki](../products/724c9add-8cd9-4013-b9e1-a907b96da426.md)
- [CrowdStrike - FDR](../products/569a3a44-c29f-492e-bcf4-5dc04e2ab0f3.md)
- [CrowdStrike - Falcon](../products/840c72e0-4e47-41e7-9b93-31f55d12f07d.md)
- [Dell - Firewall](../products/b1639f7f-4c11-4d29-ab69-368cf0e05e25.md)
- [Fortinet - Fortigate](../products/c57e2c85-4fc1-4fb7-8fa1-dbc5235231ad.md)
- [Google - Google Cloud Platform](../products/dcc85cfc-a698-4d09-87de-f2c723f3ad07.md)
- [Juniper - SRX Series Firewall](../products/A17B3F3C-04F1-40C8-9497-3C499EB18A74.md)
- [Microsoft - Azure](../products/a1225af5-e778-4068-a9a2-47da93d1ff24.md)
- [Microsoft - Defender Advanced Hunting](../products/3382523e-2072-41bd-b50b-6b148957d0b0.md)
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)
- [OISF - Suricata IDS](../products/afabb29d-e728-410f-b7c6-acfa9efbe1ed.md)
- [Palo Alto Networks - Next Generation Firewall](../products/46f5fa2c-1a62-4692-82ad-ed87800a0adb.md)
- [Palo Alto Networks - Prisma Cloud](../products/343b9323-d279-40d9-946f-809242e5cf98.md)
- [Sophos - UTM 9](../products/0fb003bc-8383-442f-8f3d-afcfbaefe617.md)
- [WatchGuard - Fireware](../products/14aa46d3-0710-44b6-9ce3-0a6b8f36b076.md)
- [Zero Networks - Segment](../products/cf2af9e8-bade-4f28-8bca-b30aa41baec4.md)
- [Zscaler - Firewall](../products/9e0641a7-22ce-4ac8-8113-ee48b368ac3d.md)
- [Zscaler - Nanolog Streaming Service](../products/6299d728-14f7-455e-85c5-ea8ec65a654a.md)


## Dynamic Signal Score/Severity Translation

The default score of `1` is used as a catch all if none of the translations are met.

|Schema Field|Field Value|Score/Severity|
|------------|-----------|--------------|
|application|irc|3|
## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|application|
|Normalized Schema|dstDevice_ip_isInternal|
|Normalized Schema|dstPort|
|Normalized Schema|listMatches|
|Normalized Schema|srcDevice_hostname|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|srcDevice_ip_isInternal|
|Normalized Schema|user_username|


