# [Rules](README.md): Potential Inbound VNC Traffic

## Description
Observes for successful TCP traffic to default VNC ports or explicit VNC/RFB traffic detected

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Unknown/Other|
|Apply Risk to Entities|dstDevice_hostname, dstDevice_ip|
|Signal Name|Potential Inbound VNC Traffic|
|Summary Expression|Potential VNC traffic detected to IP: {{dstDevice_ip}} Host: {{dstDevice_hostname}}|
|Score/Severity|Static: 1|
|Enabled by Default|False|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0008, _mitreAttackTechnique:T1021, _mitreAttackTechnique:T1021.005|
## Vendors and Products
- [Amazon AWS - VpcFlowLogs](../products/021d1ded-1c82-4663-bf5d-d6ed5170efa3.md)
- [CheckPoint - Firewall and VPN](../products/c3c1a4fc-10cc-4155-8a30-a3bb14fc9f31.md)
- [CheckPoint - SmartDefense](../products/2b82e665-bdde-474a-ae29-4f0f76598556.md)
- [Fortinet - Fortigate](../products/c57e2c85-4fc1-4fb7-8fa1-dbc5235231ad.md)
- [Palo Alto Networks - Next Generation Firewall](../products/46f5fa2c-1a62-4692-82ad-ed87800a0adb.md)
- [Sophos - UTM 9](../products/0fb003bc-8383-442f-8f3d-afcfbaefe617.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|application|
|Normalized Schema|dstDevice_hostname|
|Normalized Schema|dstDevice_ip|
|Normalized Schema|dstPort|
|Normalized Schema|ipProtocol|
|Normalized Schema|objectType|
|Normalized Schema|srcDevice_ip_isInternal|
|Normalized Schema|success|


