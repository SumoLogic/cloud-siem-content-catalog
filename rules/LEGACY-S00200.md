# [Rules](README.md): Cisco Umbrella - DNS Request Category: Phishing

## Description
Cisco Umbrella detected a DNS request to a domain categorized as Adware.

## Additional Details
|Detail|Value|
|----|----|
|Type|Match|
|Category|Initial Access|
|Apply Risk to Entities|srcDevice_ip, user_username, srcDevice_hostname|
|Signal Name|Cisco Umbrella - DNS Request Category: Phishing|
|Summary Expression|Cisco Umbrella Categorized as Phishing the URL: {{dns_query}}|
|Score/Severity|Static: 2|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0001, _mitreAttackTactic:TA0043, _mitreAttackTechnique:T1566, _mitreAttackTechnique:T1566.001, _mitreAttackTechnique:T1566.002, _mitreAttackTechnique:T1566.003, _mitreAttackTechnique:T1598, _mitreAttackTechnique:T1598.001, _mitreAttackTechnique:T1598.002, _mitreAttackTechnique:T1598.003|
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


