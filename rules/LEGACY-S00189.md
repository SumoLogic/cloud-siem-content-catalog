# [Rules](README.md): Crypto Miner HTTP User Agent

## Description
This signal looks for HTTP requests where the user agent matches common names associated with crypto miners. It is common for attackers to install crypto miners on compromised hosts to use your CPU resources for their profit.

## Additional Details
|Detail|Value|
|----|----|
|Type|Match|
|Category|Execution|
|Apply Risk to Entities|device_ip, srcDevice_ip, dstDevice_ip, device_hostname, srcDevice_hostname, dstDevice_hostname|
|Signal Name|Crypto Miner HTTP User Agent|
|Summary Expression|User agent string: {{http_userAgent}} contains keywords associated with crypto miners.|
|Score/Severity|Static: 2|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0002, _mitreAttackTactic:TA0040, _mitreAttackTechnique:T1496, _mitreAttackTechnique:T1071.001, _mitreAttackTechnique:T1071|
## Vendors and Products
- [Akamai - SIEM](../products/9a28f2af-5526-414d-973b-c3fc7984b8a1.md)
- [Akamai - Web Application Firewall](../products/ae07663e-2c2c-4932-be5d-c9f985e95276.md)
- [Amazon AWS - Application Load Balancer](../products/5bb9e0b3-8d57-4b10-8952-0b6ffe91b599.md)
- [Amazon AWS - CloudFront](../products/44f07c08-c2ad-4a95-a058-1d0737ff90db.md)
- [Amazon AWS - CloudTrail](../products/033624b0-218e-4dcb-b93f-0f1fb1806c56.md)
- [Amazon AWS - Web Application Firewall (WAF)](../products/072b85a2-1765-45c2-911d-b0509880326e.md)
- [Cloudflare - Logpush](../products/c2503fcc-ef30-4e40-bb32-0bf47151b140.md)
- [Forcepoint - Web Security](../products/e90edc67-68d4-4d67-82f6-4524f94b59bb.md)
- [Google - Google Cloud Platform](../products/dcc85cfc-a698-4d09-87de-f2c723f3ad07.md)
- [Imperva - Imperva Incapsula](../products/2a236ab1-77d2-4867-a571-a1cfd64528e6.md)
- [Microsoft - Office 365](../products/d3ed003d-5ddd-4c7a-bea5-63eae6311833.md)
- [Nginx - Nginx](../products/1ce88b4b-d90d-4d50-9a89-3abe83e8d5f8.md)
- [OISF - Suricata IDS](../products/afabb29d-e728-410f-b7c6-acfa9efbe1ed.md)
- [Okta - Single Sign-On](../products/51278354-d6b5-4c8e-a8fd-8197df334e67.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|dstDevice_hostname|
|Normalized Schema|dstDevice_ip|
|Normalized Schema|http_userAgent|
|Normalized Schema|srcDevice_hostname|
|Normalized Schema|srcDevice_ip|


