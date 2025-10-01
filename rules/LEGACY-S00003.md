# [Rules](README.md): Base32 in DNS Query

## Description
By using base32, binary and text data can be encoded in a way that is fully compliant with DNS protocol specifications.  Since common standard base32 uses 2-7 and the letters a-z, entropy must be measured to distinguish from normal text.  The presence of long base32 encoding in a DNS query may indicate tunneling of information out of a network.  Some security vendors and internet providers also use this technique to operate cloud infrastructure or transport information through firewalled environments.

## Additional Details
|Detail|Value|
|----|----|
|Type|Match|
|Category|Exfiltration|
|Apply Risk to Entities|srcDevice_ip|
|Signal Name|Base32 in DNS Query|
|Summary Expression|Base32 in DNS Query from source host: {{srcDevice_ip}}|
|Score/Severity|Static: 2|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0011, _mitreAttackTechnique:T1132.001, _mitreAttackTechnique:T1132|
## Vendors and Products
- [Amazon AWS - Route53](../products/e2393771-bda2-414a-8661-0a57069287ad.md)
- [Bro - Bro](../products/37C866BF-72E1-470A-9072-EDB908F56951.md)
- [Cisco Systems - Umbrella](../products/5ba50e74-3c05-4ea8-aeaf-5efde588c60f.md)
- [Cloudflare - Logpush](../products/c2503fcc-ef30-4e40-bb32-0bf47151b140.md)
- [Fortinet - Fortigate](../products/c57e2c85-4fc1-4fb7-8fa1-dbc5235231ad.md)
- [ISC - Bind](../products/1768a42a-37e6-4a2b-aa42-314583f63e1b.md)
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)
- [Netskope - WebTx](../products/9e838f93-c9e7-4592-a980-cf9dfb704784.md)
- [Zscaler - Firewall](../products/9e0641a7-22ce-4ac8-8113-ee48b368ac3d.md)
- [Zscaler - Nanolog Streaming Service](../products/6299d728-14f7-455e-85c5-ea8ec65a654a.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|dns_query|
|Normalized Schema|dns_queryDomain_alexaRank|
|Normalized Schema|dns_queryDomain_entropyFqdn|
|Normalized Schema|listMatches|
|Normalized Schema|srcDevice_ip|


