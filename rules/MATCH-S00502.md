# [Rules](README.md): RDP Traffic to Unexpected Host

## Description
Observes for RDP traffic to hosts not within an allow list.

Note that this rule requires the creation and population of a match list for known OK hosts named 'RDP_Hosts'

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Lateral Movement|
|Apply Risk to Entities|srcDevice_hostname, srcDevice_ip, user_username|
|Signal Name|RDP Traffic to Unexpected Host|
|Summary Expression|RDP connection from IP: {{srcDevice_ip}} to IP: {{dstDevice_ip}}|
|Score/Severity|Static: 1|
|Enabled by Default|False|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0008, _mitreAttackTactic:TA0011, _mitreAttackTechnique:T1219, _mitreAttackTechnique:T1021.001, _mitreAttackTechnique:T1021|
## Vendors and Products
- [Amazon AWS - Network Firewall](../products/3a82061c-2ca3-4289-9c9b-78756001aa38.md)
- [Amazon AWS - VpcFlowLogs](../products/021d1ded-1c82-4663-bf5d-d6ed5170efa3.md)
- [CheckPoint - Firewall and VPN](../products/c3c1a4fc-10cc-4155-8a30-a3bb14fc9f31.md)
- [CheckPoint - SmartDefense](../products/2b82e665-bdde-474a-ae29-4f0f76598556.md)
- [Cisco Systems - ASA](../products/be4f7473-fe69-4311-8859-3561900060bf.md)
- [Cisco Systems - Meraki](../products/724c9add-8cd9-4013-b9e1-a907b96da426.md)
- [Citrix - ADC](../products/d3606245-76d3-4173-a2fe-832c0e71b0f9.md)
- [Fortinet - Fortigate](../products/c57e2c85-4fc1-4fb7-8fa1-dbc5235231ad.md)
- [Juniper - SRX Series Firewall](../products/A17B3F3C-04F1-40C8-9497-3C499EB18A74.md)
- [Microsoft - Azure](../products/a1225af5-e778-4068-a9a2-47da93d1ff24.md)
- [Microsoft - Defender Advanced Hunting](../products/3382523e-2072-41bd-b50b-6b148957d0b0.md)
- [Palo Alto Networks - Next Generation Firewall](../products/46f5fa2c-1a62-4692-82ad-ed87800a0adb.md)
- [Sophos - UTM 9](../products/0fb003bc-8383-442f-8f3d-afcfbaefe617.md)
- [Symantec - Endpoint Protection](../products/eb2f69a8-8d13-447f-9859-1ad0979b4a24.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|dstDevice_hostname|
|Normalized Schema|dstDevice_ip_isInternal|
|Normalized Schema|dstPort|
|Normalized Schema|listMatches|
|Normalized Schema|srcDevice_hostname|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|success|
|Normalized Schema|user_username|


