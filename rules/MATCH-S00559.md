# [Rules](README.md): Traffic to Honeypot IP

## Description
This rule monitors for traffic being sent to a honeypot, indicating an attacker may be on the network attempting to move laterally. Requires configuration of the honeypot_ip_addresses list in order to function.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Unknown/Other|
|Apply Risk to Entities|srcDevice_ip, srcDevice_hostname|
|Signal Name|Traffic to Honeypot IP|
|Summary Expression|Source IP {{srcDevice_ip}} was observed attempting to communicate with known honeypot {{dstDevice_ip}} .|
|Score/Severity|Static: 6|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0011, _mitreAttackTechnique:T1071, _mitreAttackTechnique:T1071.001|
## Vendors and Products
- [Fortinet - Fortigate](../products/c57e2c85-4fc1-4fb7-8fa1-dbc5235231ad.md)
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)
- [Palo Alto Networks - Next Generation Firewall](../products/46f5fa2c-1a62-4692-82ad-ed87800a0adb.md)
- [Zero Networks - Segment](../products/cf2af9e8-bade-4f28-8bca-b30aa41baec4.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|srcDevice_hostname|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|srcDevice_ip_isInternal|


