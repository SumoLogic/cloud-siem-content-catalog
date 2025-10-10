# [Rules](README.md): Suspicious HTTP User-Agent

## Description
Common administrative tools may be used by malware authors and attackers who use live-off-the-land methods to operate on victim networks.

## Additional Details
|Detail|Value|
|----|----|
|Type|Match|
|Category|Execution|
|Apply Risk to Entities|device_ip, srcDevice_ip, dstDevice_ip, device_hostname, srcDevice_hostname, dstDevice_hostname, user_username, dstDevice_hostname, dstDevice_ip|
|Signal Name|Suspicious HTTP User-Agent|
|Summary Expression|Suspicious user agent from IP: {{srcDevice_ip}} user agent: {{http_userAgent}}|
|Score/Severity|Static: 1|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0002, _mitreAttackTactic:TA0004, _mitreAttackTactic:TA0005, _mitreAttackTactic:TA0007, _mitreAttackTactic:TA0011, _mitreAttackTechnique:T1059, _mitreAttackTechnique:T1059.003, _mitreAttackTechnique:T1059.001, _mitreAttackTechnique:T1083, _mitreAttackTechnique:T1132, _mitreAttackTechnique:T1548, _mitreAttackTactic:TA0009, _mitreAttackTechnique:T1213, _mitreAttackTechnique:T1213.001|
## Vendors and Products
- [Akamai - SIEM](../products/9a28f2af-5526-414d-973b-c3fc7984b8a1.md)
- [Amazon AWS - API Gateway](../products/9f76f1fd-fbb0-42d2-9bf5-0f4fd2c1ab82.md)
- [Amazon AWS - Application Load Balancer](../products/5bb9e0b3-8d57-4b10-8952-0b6ffe91b599.md)
- [Amazon AWS - CloudFront](../products/44f07c08-c2ad-4a95-a058-1d0737ff90db.md)
- [Amazon AWS - CloudTrail](../products/033624b0-218e-4dcb-b93f-0f1fb1806c56.md)
- [Amazon AWS - EKS](../products/234ec2b5-4142-4837-bc78-95da8a2db81a.md)
- [Amazon AWS - Elastic Load Balancer](../products/59a3cd41-b6d2-4ab7-a0ff-6d5abd14ac43.md)
- [Amazon AWS - Web Application Firewall (WAF)](../products/072b85a2-1765-45c2-911d-b0509880326e.md)
- [Apache - Apache HTTP Server](../products/6787d77a-1ee0-43d4-8ca0-96af8ee755bc.md)
- [Barracuda - Web Application Firewall](../products/798f8da8-c85b-4e9a-b2f1-eae0b07532fb.md)
- [Bro - Bro](../products/37C866BF-72E1-470A-9072-EDB908F56951.md)
- [Cisco Systems - Firepower](../products/da9e05a5-3fd3-46a7-a107-ae03c01e3f5a.md)
- [Cisco Systems - Meraki](../products/724c9add-8cd9-4013-b9e1-a907b96da426.md)
- [Cisco Systems - Umbrella](../products/5ba50e74-3c05-4ea8-aeaf-5efde588c60f.md)
- [Cloudflare - Logpush](../products/c2503fcc-ef30-4e40-bb32-0bf47151b140.md)
- [Forcepoint - Web Security](../products/e90edc67-68d4-4d67-82f6-4524f94b59bb.md)
- [Fortinet - Fortigate](../products/c57e2c85-4fc1-4fb7-8fa1-dbc5235231ad.md)
- [Google - Google Cloud Platform](../products/dcc85cfc-a698-4d09-87de-f2c723f3ad07.md)
- [Imperva - Imperva Incapsula](../products/2a236ab1-77d2-4867-a571-a1cfd64528e6.md)
- [JFrog - Artifactory](../products/abe4975e-de65-4f82-8b35-e6ce392e165c.md)
- [McAfee - Web Gateway](../products/003d35b3-3ba8-4e93-8776-e5810b4e243e.md)
- [Microsoft - Azure](../products/a1225af5-e778-4068-a9a2-47da93d1ff24.md)
- [Microsoft - Defender Advanced Hunting](../products/3382523e-2072-41bd-b50b-6b148957d0b0.md)
- [Microsoft - IIS](../products/fca8785d-4823-4442-86b2-8acbaa176da4.md)
- [Microsoft - Office 365](../products/d3ed003d-5ddd-4c7a-bea5-63eae6311833.md)
- [Netskope - Security Cloud](../products/B3582ED2-1A0C-452D-9802-97433D143486.md)
- [Netskope - WebTx](../products/9e838f93-c9e7-4592-a980-cf9dfb704784.md)
- [OISF - Suricata IDS](../products/afabb29d-e728-410f-b7c6-acfa9efbe1ed.md)
- [Okta - Single Sign-On](../products/51278354-d6b5-4c8e-a8fd-8197df334e67.md)
- [Palo Alto Networks - Next Generation Firewall](../products/46f5fa2c-1a62-4692-82ad-ed87800a0adb.md)
- [Signal Sciences - Web Application Firewall](../products/2f2fbe08-ab8b-4626-81fd-eaa41b563c49.md)
- [Sophos - UTM 9](../products/0fb003bc-8383-442f-8f3d-afcfbaefe617.md)
- [Symantec - Proxy Secure Gateway](../products/991a55cf-8c5a-49ba-ae72-6f64a002bacf.md)
- [Zscaler - Firewall](../products/9e0641a7-22ce-4ac8-8113-ee48b368ac3d.md)
- [Zscaler - Nanolog Streaming Service](../products/6299d728-14f7-455e-85c5-ea8ec65a654a.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|dstDevice_hostname|
|Normalized Schema|dstDevice_ip|
|Normalized Schema|http_url_path|
|Normalized Schema|http_userAgent|
|Normalized Schema|listMatches|
|Normalized Schema|lower|
|Normalized Schema|srcDevice_hostname|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|user_username|


