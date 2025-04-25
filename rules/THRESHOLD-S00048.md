# [Rules](README.md): Outbound Traffic to Countries Outside the United States

## Description
Traffic was observed leaving your network destined to some countries outside the United States within a time frame. This rule is shipped disabled by default as is intended for environments based in the United States with very tight network restriction policies. 

## Additional Details
|Detail|Value|
|----|----|
|Type|Threshold|
|Category|Unknown/Other|
|Apply Risk to Entities|device_ip, user_username, device_hostname, srcDevice_ip|
|Signal Name|Outbound Traffic to Countries Outside the United States|
|Summary Expression|Traffic to countries outside the United States|
|Threshold Count|2|
|Threshold Window|30m|
|Score/Severity|Static: 1|
|Enabled by Default|False|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0011, _mitreAttackTechnique:T1071, _mitreAttackTechnique:T1071.001|
## Vendors and Products
- [Amazon AWS - VpcFlowLogs](../products/021d1ded-1c82-4663-bf5d-d6ed5170efa3.md)
- [Bro - Bro](../products/37C866BF-72E1-470A-9072-EDB908F56951.md)
- [CheckPoint - Application Control](../products/1624169f-36c4-4309-8400-1409a171d00b.md)
- [CheckPoint - Firewall and VPN](../products/c3c1a4fc-10cc-4155-8a30-a3bb14fc9f31.md)
- [CheckPoint - SmartDefense](../products/2b82e665-bdde-474a-ae29-4f0f76598556.md)
- [CheckPoint - URL Filtering](../products/2a678bcd-898e-43cd-ab3f-91feb0602a18.md)
- [Cisco Systems - ASA](../products/be4f7473-fe69-4311-8859-3561900060bf.md)
- [Cisco Systems - Meraki](../products/724c9add-8cd9-4013-b9e1-a907b96da426.md)
- [Cisco Systems - Umbrella](../products/5ba50e74-3c05-4ea8-aeaf-5efde588c60f.md)
- [Fortinet - Fortigate](../products/c57e2c85-4fc1-4fb7-8fa1-dbc5235231ad.md)
- [Juniper - SRX Series Firewall](../products/A17B3F3C-04F1-40C8-9497-3C499EB18A74.md)
- [Microsoft - Defender Advanced Hunting](../products/3382523e-2072-41bd-b50b-6b148957d0b0.md)
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)
- [OISF - Suricata IDS](../products/afabb29d-e728-410f-b7c6-acfa9efbe1ed.md)
- [Palo Alto Networks - Next Generation Firewall](../products/46f5fa2c-1a62-4692-82ad-ed87800a0adb.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|dstDevice_ip_countryCode|
|Normalized Schema|dstDevice_ip_isInternal|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|srcDevice_ip_isInternal|
|Normalized Schema|user_username|


