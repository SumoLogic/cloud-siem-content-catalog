# [Rules](README.md): Domain Resolution in Non-Standard TLD

## Description
DNS resolution of a domain that is not under an ICANN-standard TLD. These TLDs are provided by alternate DNS root servers such as OpenNIC. Their use on corporate networks is fundamentally suspicious and potentially a sign of abuse by threat actors.

## Additional Details
|Detail|Value|
|----|----|
|Type|Match|
|Category|Command and Control|
|Apply Risk to Entities|srcDevice_ip|
|Signal Name|Domain Resolution in Non-Standard TLD|
|Summary Expression|Non-Standard TLD detected in URL: {{dns_queryDomain}}|
|Score/Severity|Static: 6|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0011, _mitreAttackTechnique:T1568, _mitreAttackTechnique:T1568.001, _mitreAttackTechnique:T1568.002, _mitreAttackTechnique:T1568.003|
## Vendors and Products
- [Amazon AWS - Route53](../products/e2393771-bda2-414a-8661-0a57069287ad.md)
- [Bro - Bro](../products/37C866BF-72E1-470A-9072-EDB908F56951.md)
- [Cisco Systems - Umbrella](../products/5ba50e74-3c05-4ea8-aeaf-5efde588c60f.md)
- [Fortinet - Fortigate](../products/c57e2c85-4fc1-4fb7-8fa1-dbc5235231ad.md)
- [Google - Google Cloud Platform](../products/dcc85cfc-a698-4d09-87de-f2c723f3ad07.md)
- [ISC - Bind](../products/1768a42a-37e6-4a2b-aa42-314583f63e1b.md)
- [Infoblox - Network Identity Operating System](../products/43808f4c-15e9-480c-ab1a-38bdef3b6798.md)
- [Microsoft - Azure](../products/a1225af5-e778-4068-a9a2-47da93d1ff24.md)
- [Zscaler - Firewall](../products/9e0641a7-22ce-4ac8-8113-ee48b368ac3d.md)
- [Zscaler - Nanolog Streaming Service](../products/6299d728-14f7-455e-85c5-ea8ec65a654a.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|dns_queryDomain_tld|
|Normalized Schema|listMatches|
|Normalized Schema|srcDevice_ip|


