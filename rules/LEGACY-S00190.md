# [Rules](README.md): Cisco Umbrella - DNS Request Category: Adware

## Description
Cisco Umbrella detected a DNS request to a domain categorized as Adware.

## Additional Details
|Detail|Value|
|----|----|
|Type|Match|
|Category|Collection|
|Apply Risk to Entities|srcDevice_ip, user_username, srcDevice_hostname|
|Signal Name|Cisco Umbrella - DNS Request Category: Adware|
|Summary Expression|Cisco Umbrealla Categorized as Adware the URL: {{dns_query}}|
|Score/Severity|Static: 1|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0011, _mitreAttackTechnique:T1071, _mitreAttackTechnique:T1071.004|
## Vendors and Products
- [Cisco Systems - Umbrella](../products/5ba50e74-3c05-4ea8-aeaf-5efde588c60f.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|http_category|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|srcDevice_hostname|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|user_username|


