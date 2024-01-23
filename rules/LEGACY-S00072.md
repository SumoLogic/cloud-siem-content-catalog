# [Rules](README.md): Request to DNS over HTTPS (DoH) Service Provider

## Description
DNS over HTTPS (RFC 8484, DoH) is a web based name resolution service that allows clients to resolve DNS records over web services. DoH operates over standards compliant HTTPS and is therefore typically encrypted and validated TLS over port 443/tcp. In some environments this may be abused as a method to bypass security and policy controls. Some malicious actors leverage DoH to tunnel DNS traffic over HTTPS, and research has demonstrated the ability to carry out other DNS related abuse such as malware C2 over DoH as well.

## Additional Details
|Detail|Value|
|----|----|
|Type|Match|
|Category|Defense Evasion|
|Apply Risk to Entities|device_hostname, device_ip, srcDevice_hostname, srcDevice_ip, user_username|
|Signal Name|Request to DNS over HTTPS (DoH) Service Provider|
|Summary Expression|Request to DNS over HTTPS provider from IP: {{srcDevice_ip}} to IP: {{dstDevice_ip}}|
|Score/Severity|Static: 1|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0005, _mitreAttackTactic:TA0011, _mitreAttackTechnique:T1071, _mitreAttackTechnique:T1071.004|
## Vendors and Products
- [Bro - Bro](../products/37C866BF-72E1-470A-9072-EDB908F56951.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|bro_ssl_serverName|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|srcDevice_hostname|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|user_username|


