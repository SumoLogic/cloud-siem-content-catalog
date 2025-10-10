# [Rules](README.md): First Seen SMB Allowed Traffic From IP

## Description
Observes for SMB traffic allowed through the firewall.

## Additional Details
|Detail|Value|
|----|----|
|Type|First Seen|
|Category|Lateral Movement|
|Apply Risk to Entities|srcDevice_ip|
|Signal Name|First Seen SMB Allowed Traffic From IP|
|Summary Expression|First seen allowed SMB traffic from IP {{srcDevice_ip}} to {{dstDevice_ip}}|
|Retention Window|7776000000|
|Baseline Window|3024000000|
|Baseline Type|GLOBAL|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0008, _mitreAttackTechnique:T1210|
## Vendors and Products
- [Amazon AWS - VpcFlowLogs](../products/021d1ded-1c82-4663-bf5d-d6ed5170efa3.md)
- [CheckPoint - Application Control](../products/1624169f-36c4-4309-8400-1409a171d00b.md)
- [CheckPoint - Firewall and VPN](../products/c3c1a4fc-10cc-4155-8a30-a3bb14fc9f31.md)
- [Cisco Systems - Firepower](../products/da9e05a5-3fd3-46a7-a107-ae03c01e3f5a.md)
- [Cisco Systems - Meraki](../products/724c9add-8cd9-4013-b9e1-a907b96da426.md)
- [Cloudflare - Logpush](../products/c2503fcc-ef30-4e40-bb32-0bf47151b140.md)
- [CrowdStrike - Falcon](../products/840c72e0-4e47-41e7-9b93-31f55d12f07d.md)
- [Fortinet - Fortigate](../products/c57e2c85-4fc1-4fb7-8fa1-dbc5235231ad.md)
- [Google - Google Cloud Platform](../products/dcc85cfc-a698-4d09-87de-f2c723f3ad07.md)
- [Microsoft - Azure](../products/a1225af5-e778-4068-a9a2-47da93d1ff24.md)
- [Palo Alto Networks - Next Generation Firewall](../products/46f5fa2c-1a62-4692-82ad-ed87800a0adb.md)
- [Palo Alto Networks - Prisma Cloud](../products/343b9323-d279-40d9-946f-809242e5cf98.md)
- [WatchGuard - Fireware](../products/14aa46d3-0710-44b6-9ce3-0a6b8f36b076.md)
- [Zscaler - Firewall](../products/9e0641a7-22ce-4ac8-8113-ee48b368ac3d.md)
- [Zscaler - Nanolog Streaming Service](../products/6299d728-14f7-455e-85c5-ea8ec65a654a.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|action|
|Normalized Schema|application|
|Normalized Schema|dstDevice_ip_isInternal|
|Normalized Schema|dstPort|
|Normalized Schema|ipProtocol|
|Normalized Schema|objectType|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|srcDevice_ip_isInternal|
|Normalized Schema|tcpProtocol|


