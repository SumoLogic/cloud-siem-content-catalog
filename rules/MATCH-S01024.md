# [Rules](README.md): Threat Intel - Destination IP Address (High Confidence)

## Description
This rule detects traffic to IP address with a high confidence rating from a threat intelligence feed.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Threat Intelligence|
|Apply Risk to Entities|srcDevice_ip, dstDevice_ip, device_ip, srcDevice_ip, srcDevice_hostname, srcDevice_hostname, dstDevice_hostname, device_hostname, user_username|
|Signal Name|Threat Intel - High Confidence Threat Intel Match on Destination IP Address|
|Summary Expression|The record contains a matching destination IP address from a threat intelligence feed: {{dstDevice_ip}}|
|Score/Severity|Static: 1|
|Enabled by Default|True|
|Prototype|False|
|Tags||
## Vendors and Products
- [Amazon AWS - Network Firewall](../products/3a82061c-2ca3-4289-9c9b-78756001aa38.md)
- [Amazon AWS - VpcFlowLogs](../products/021d1ded-1c82-4663-bf5d-d6ed5170efa3.md)
- [CheckPoint - Firewall and VPN](../products/c3c1a4fc-10cc-4155-8a30-a3bb14fc9f31.md)
- [Cisco Systems - ASA](../products/be4f7473-fe69-4311-8859-3561900060bf.md)
- [Cisco Systems - Meraki](../products/724c9add-8cd9-4013-b9e1-a907b96da426.md)
- [Fortinet - Fortigate](../products/c57e2c85-4fc1-4fb7-8fa1-dbc5235231ad.md)
- [Illumio - Adaptive Security Platform](../products/1afb4979-e858-43fe-8a55-87f444f0417b.md)
- [Netskope - Security Cloud](../products/B3582ED2-1A0C-452D-9802-97433D143486.md)
- [Palo Alto Networks - Next Generation Firewall](../products/46f5fa2c-1a62-4692-82ad-ed87800a0adb.md)
- [Pfsense - Pfsense Firewall](../products/ef11c9cd-df72-42c6-81f5-70b91fd0f38a.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|OR|
|Normalized Schema|confidence|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|dstDevice_hostname|
|Normalized Schema|dstDevice_ip|
|Normalized Schema|listMatches|
|Normalized Schema|srcDevice_hostname|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|type|
|Normalized Schema|user_username|


