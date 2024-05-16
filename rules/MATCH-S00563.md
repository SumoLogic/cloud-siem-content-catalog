# [Rules](README.md): Traffic to Proxy Anonymizers

## Description
Observes for outbound traffic to a proxy anonymizer. This rule requires a list populated with IP addresses of known proxy anonymizers.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Unknown/Other|
|Apply Risk to Entities|srcDevice_ip, user_username|
|Signal Name|Traffic to Proxy Anonymizers|
|Summary Expression|Detected proxy anonymizer traffic from IP: {{srcDevice_ip}}  User: {{user_username}}|
|Score/Severity|Static: 1|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0011, _mitreAttackTechnique:T1090, _mitreAttackTechnique:T1090.002, _mitreAttackTechnique:T1090.003|
## Vendors and Products
- [Fortinet - Fortigate](../products/c57e2c85-4fc1-4fb7-8fa1-dbc5235231ad.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|dstDevice_ip|
|Normalized Schema|listMatches|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|success|
|Normalized Schema|user_username|


