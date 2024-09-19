# [Rules](README.md): Critical Severity Intrusion Signature

## Description
This rule looks for an intrusion product detecting a critical severity intrusion signature sourcing from an internal IP.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Discovery|
|Apply Risk to Entities|srcDevice_hostname, srcDevice_ip, user_username|
|Signal Name|{{metadata_vendor}} {{metadata_product}} Critical Severity Intrusion Signature - {{threat_name}}|
|Summary Expression|Detected a critical severity intrusion: {{threat_name}} from IP: {{srcDevice_ip}}|
|Score/Severity|Static: 4|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0007, _mitreAttackTechnique:T1046|
## Vendors and Products
- [Amazon AWS - Network Firewall](../products/3a82061c-2ca3-4289-9c9b-78756001aa38.md)
- [Cisco Systems - ASA](../products/be4f7473-fe69-4311-8859-3561900060bf.md)
- [Cisco Systems - Firepower](../products/da9e05a5-3fd3-46a7-a107-ae03c01e3f5a.md)
- [Cisco Systems - Meraki](../products/724c9add-8cd9-4013-b9e1-a907b96da426.md)
- [Fortinet - Fortigate](../products/c57e2c85-4fc1-4fb7-8fa1-dbc5235231ad.md)
- [Google - Security Command Center](../products/78a80406-d37b-4a17-a25e-dbf53289b647.md)
- [OISF - Suricata IDS](../products/afabb29d-e728-410f-b7c6-acfa9efbe1ed.md)
- [Palo Alto Networks - Next Generation Firewall](../products/46f5fa2c-1a62-4692-82ad-ed87800a0adb.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|dstDevice_hostname|
|Normalized Schema|listMatches|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|normalizedSeverity|
|Normalized Schema|srcDevice_hostname|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|srcDevice_ip_isInternal|
|Normalized Schema|threat_name|
|Normalized Schema|threat_ruleType|
|Normalized Schema|user_username|


