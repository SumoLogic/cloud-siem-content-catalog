# [Rules](README.md): DNS Lookup of High Entropy Domain

## Description
DNS lookup of a high entropy domain name, which may be indicative of a domain generation algorithm (DGA) related domain.  This technique is described at https://attack.mitre.org/techniques/T1483/.

## Additional Details
|Detail|Value|
|----|----|
|Type|Match|
|Category|Exfiltration|
|Apply Risk to Entities|srcDevice_ip|
|Signal Name|DNS Lookup of High Entropy Domain|
|Summary Expression|High entropy domain: {{dns_queryDomain_rootDomain}}|
|Score/Severity|Static: 2|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0010, _mitreAttackTactic:TA0011, _mitreAttackTechnique:T1568, _mitreAttackTechnique:T1568.002|
## Vendors and Products
- [Amazon AWS - Application Load Balancer](../products/5bb9e0b3-8d57-4b10-8952-0b6ffe91b599.md)
- [Amazon AWS - Route53](../products/e2393771-bda2-414a-8661-0a57069287ad.md)
- [Amazon AWS - Web Application Firewall (WAF)](../products/072b85a2-1765-45c2-911d-b0509880326e.md)
- [Bro - Bro](../products/37C866BF-72E1-470A-9072-EDB908F56951.md)
- [Cisco Systems - Umbrella](../products/5ba50e74-3c05-4ea8-aeaf-5efde588c60f.md)
- [Cloudflare - Logpush](../products/c2503fcc-ef30-4e40-bb32-0bf47151b140.md)
- [Fortinet - Fortigate](../products/c57e2c85-4fc1-4fb7-8fa1-dbc5235231ad.md)
- [Google - Google Cloud Platform](../products/dcc85cfc-a698-4d09-87de-f2c723f3ad07.md)
- [Infoblox - Network Identity Operating System](../products/43808f4c-15e9-480c-ab1a-38bdef3b6798.md)
- [Microsoft - Azure](../products/a1225af5-e778-4068-a9a2-47da93d1ff24.md)
- [Microsoft - DNS](../products/e362ae18-9af1-496d-9ace-efa05a8381c6.md)
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)
- [Netskope - WebTx](../products/9e838f93-c9e7-4592-a980-cf9dfb704784.md)
- [Sophos - UTM 9](../products/0fb003bc-8383-442f-8f3d-afcfbaefe617.md)
- [WatchGuard - Fireware](../products/14aa46d3-0710-44b6-9ce3-0a6b8f36b076.md)
- [Zscaler - Firewall](../products/9e0641a7-22ce-4ac8-8113-ee48b368ac3d.md)
- [Zscaler - Nanolog Streaming Service](../products/6299d728-14f7-455e-85c5-ea8ec65a654a.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|dns_queryDomain_alexaRank|
|Normalized Schema|dns_queryDomain_entropyRootDomain|
|Normalized Schema|listMatches|
|Normalized Schema|srcDevice_ip|


