# [Rules](README.md): Cisco Stealthwatch Template Alerts

## Description
Passthrough alerts from Cisco Stealthwatch

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Unknown/Other|
|Apply Risk to Entities|srcDevice_ip|
|Signal Name|Cisco Stealthwatch - {{fields['cat']}}|
|Summary Expression|{{fields['fullmessage']}}|
|Score/Severity|Static: 1|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0001, _mitreAttackTechnique:T1190|
## Vendors and Products
- [Cisco Systems - Stealthwatch](../products/8a30c984-6d57-4959-ae04-1d6f5156b4bf.md)


## Fields Used

|Origin|Field|
|----|----|
|Direct from Record|fields['cat']|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|srcDevice_ip|


