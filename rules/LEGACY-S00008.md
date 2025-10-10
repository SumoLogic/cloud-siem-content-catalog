# [Rules](README.md): Possible Dynamic DNS Domain

## Description
This rule looks for DNS query/reply domains which appear to be associated with a dynamic DNS service.

## Additional Details
|Detail|Value|
|----|----|
|Type|Match|
|Category|Command and Control|
|Apply Risk to Entities|device_hostname, device_ip, srcDevice_hostname, srcDevice_ip, user_username|
|Signal Name|Possible Dynamic DNS Domain|
|Summary Expression|Possible dynamic DNS domain for URL: {{dns_queryDomain}}|
|Score/Severity|Static: 1|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0011, _mitreAttackTechnique:T1568, _mitreAttackTechnique:T1568.001, _mitreAttackTechnique:T1568.002, _mitreAttackTechnique:T1568.003|
## Vendors and Products
- [Amazon AWS - Application Load Balancer](../products/5bb9e0b3-8d57-4b10-8952-0b6ffe91b599.md)
- [Amazon AWS - Route53](../products/e2393771-bda2-414a-8661-0a57069287ad.md)
- [Amazon AWS - Web Application Firewall (WAF)](../products/072b85a2-1765-45c2-911d-b0509880326e.md)
- [Bro - Bro](../products/37C866BF-72E1-470A-9072-EDB908F56951.md)
- [Cisco Systems - Umbrella](../products/5ba50e74-3c05-4ea8-aeaf-5efde588c60f.md)
- [Cloudflare - Logpush](../products/c2503fcc-ef30-4e40-bb32-0bf47151b140.md)
- [CrowdStrike - FDR](../products/569a3a44-c29f-492e-bcf4-5dc04e2ab0f3.md)
- [Fortinet - Fortigate](../products/c57e2c85-4fc1-4fb7-8fa1-dbc5235231ad.md)
- [Google - BigQuery](../products/a67d97fe-6e68-4cfb-9500-cfc5492da565.md)
- [ISC - Bind](../products/1768a42a-37e6-4a2b-aa42-314583f63e1b.md)
- [Infoblox - Network Identity Operating System](../products/43808f4c-15e9-480c-ab1a-38bdef3b6798.md)
- [Microsoft - DNS](../products/e362ae18-9af1-496d-9ace-efa05a8381c6.md)
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)
- [Netskope - WebTx](../products/9e838f93-c9e7-4592-a980-cf9dfb704784.md)
- [Sophos - UTM 9](../products/0fb003bc-8383-442f-8f3d-afcfbaefe617.md)
- [WatchGuard - Fireware](../products/14aa46d3-0710-44b6-9ce3-0a6b8f36b076.md)
- [Zscaler - Firewall](../products/9e0641a7-22ce-4ac8-8113-ee48b368ac3d.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|dns_queryDomain_alexaRank|
|Normalized Schema|dns_queryDomain_possibleDynDns|
|Normalized Schema|dns_replyDomain_alexaRank|
|Normalized Schema|dns_replyDomain_possibleDynDns|
|Normalized Schema|srcDevice_hostname|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|user_username|


