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
- [Amazon AWS - CloudFront](../products/44f07c08-c2ad-4a95-a058-1d0737ff90db.md)
- [Amazon AWS - CloudTrail](../products/033624b0-218e-4dcb-b93f-0f1fb1806c56.md)
- [Amazon AWS - Web Application Firewall (WAF)](../products/072b85a2-1765-45c2-911d-b0509880326e.md)
- [Cloudflare - Logpush](../products/c2503fcc-ef30-4e40-bb32-0bf47151b140.md)
- [Forcepoint - Web Security](../products/e90edc67-68d4-4d67-82f6-4524f94b59bb.md)
- [Microsoft - IIS](../products/fca8785d-4823-4442-86b2-8acbaa176da4.md)


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


