# [Rules](README.md): DNS query for dynamic DNS provider

## Description
Dynamic DNS providers are often abused to host malware control servers and other malicious content. https://attack.mitre.org/techniques/T1311/ and https://attack.mitre.org/techniques/T1333/ describe the use of this technique by attackers.

## Additional Details
|Detail|Value|
|----|----|
|Type|Match|
|Category|Command and Control|
|Apply Risk to Entities|srcDevice_ip|
|Signal Name|DNS query for dynamic DNS provider|
|Summary Expression|Dynamic DNS provider: {{dns_queryDomain}} detected|
|Score/Severity|Static: 2|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0011, _mitreAttackTechnique:T1568, _mitreAttackTechnique:T1568.001, _mitreAttackTechnique:T1568.002, _mitreAttackTechnique:T1568.003|
## Vendors and Products
- [Amazon AWS - Application Load Balancer](../products/5bb9e0b3-8d57-4b10-8952-0b6ffe91b599.md)
- [Bro - Bro](../products/37C866BF-72E1-470A-9072-EDB908F56951.md)
- [Cisco Systems - Umbrella](../products/5ba50e74-3c05-4ea8-aeaf-5efde588c60f.md)
- [Netskope - Security Cloud](../products/B3582ED2-1A0C-452D-9802-97433D143486.md)
- [Sophos - UTM 9](../products/0fb003bc-8383-442f-8f3d-afcfbaefe617.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|dns_query|
|Normalized Schema|dns_queryDomain|
|Normalized Schema|dns_queryDomain_rootDomain|
|Normalized Schema|listMatches|
|Normalized Schema|srcDevice_ip|


