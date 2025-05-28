# [Rules](README.md): Traffic From Embargoed Countries

## Description
Observes for traffic originating from an embargoed country. As embargoes vary from country to country, a match list must be populated with embargoed countries.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Unknown/Other|
|Apply Risk to Entities|srcDevice_ip|
|Signal Name|Traffic From Embargo Country|
|Summary Expression|Allowed traffic detected from {{srcDevice_ip_countryName}}|
|Score/Severity|Static: 4|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0011, _mitreAttackTechnique:T1071, _mitreAttackTechnique:T1071.001|
## Vendors and Products
- [Fortinet - Fortigate](../products/c57e2c85-4fc1-4fb7-8fa1-dbc5235231ad.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|dstDevice_ip_isInternal|
|Normalized Schema|listMatches|
|Normalized Schema|objectType|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|success|


