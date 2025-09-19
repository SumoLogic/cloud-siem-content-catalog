# [Rules](README.md): Direct Outbound DNS Traffic

## Description
This rule detects DNS traffic sent directly to an external server from an internal host, bypassing the existing DNS structure. This could indicate an attacker attempting to conduct command and control without being subjected to DNS monitoring.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Unknown/Other|
|Apply Risk to Entities|srcDevice_ip|
|Signal Name|Direct Outbound DNS Traffic|
|Summary Expression|Source IP {{srcDevice_ip}} was observed sending DNS traffic directly to destination IP {{dstDevice_ip}}|
|Score/Severity|Static: 1|
|Enabled by Default|False|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0011, _mitreAttackTechnique:T1071, _mitreAttackTechnique:T1071.004|
## Vendors and Products
- [Fortinet - Fortigate](../products/c57e2c85-4fc1-4fb7-8fa1-dbc5235231ad.md)
- [Palo Alto Networks - Next Generation Firewall](../products/46f5fa2c-1a62-4692-82ad-ed87800a0adb.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|application|
|Normalized Schema|listMatches|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|srcDevice_ip_isInternal|


