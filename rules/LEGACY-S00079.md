# [Rules](README.md): SQL-Select-From

## Description
Requests to web applications containing SQL statement keywords may indicate attempts to compromise the web application or access data in a backend database engine in an unauthorized manner. This technique is described at https://attack.mitre.org/techniques/T1190/.

## Additional Details
|Detail|Value|
|----|----|
|Type|Match|
|Category|Initial Access|
|Apply Risk to Entities|device_hostname, device_ip, srcDevice_hostname, srcDevice_ip, user_username|
|Signal Name|SQL-Select-From|
|Summary Expression|Web request with SQL keywords detected from IP: {{srcDevice_ip}}|
|Score/Severity|Static: 2|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0001, _mitreAttackTechnique:T1190|
## Vendors and Products
- [Amazon AWS - CloudFront](../products/44f07c08-c2ad-4a95-a058-1d0737ff90db.md)
- [Amazon AWS - Web Application Firewall (WAF)](../products/072b85a2-1765-45c2-911d-b0509880326e.md)
- [Bro - Bro](../products/37C866BF-72E1-470A-9072-EDB908F56951.md)
- [Cloudflare - Logpush](../products/c2503fcc-ef30-4e40-bb32-0bf47151b140.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|dstDevice_ip|
|Normalized Schema|http_url_path|
|Normalized Schema|listMatches|
|Normalized Schema|srcDevice_hostname|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|user_username|


