# [Rules](README.md): Shellshock

## Description
HTTP requests with headers indicating an attempt to exploit CVE-2014-6271 and related vulnerabilities in the Bash shell using Bashdoor/Shellshock attack. This vulnerability is most often triggered in CGI scripts implemented against vulnerable versions of the shell.

## Additional Details
|Detail|Value|
|----|----|
|Type|Match|
|Category|Initial Access|
|Apply Risk to Entities|device_hostname, device_ip, srcDevice_hostname, srcDevice_ip, user_username|
|Signal Name|Shellshock|
|Summary Expression|Vulnerability exploit attempted against IP: {{dstDevice_ip}}|
|Score/Severity|Static: 6|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0001, _mitreAttackTactic:TA0042, _mitreAttackTechnique:T1190|
## Vendors and Products
- [Bro - Bro](../products/37C866BF-72E1-470A-9072-EDB908F56951.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|dstDevice_ip|
|Normalized Schema|dstDevice_ip_isInternal|
|Normalized Schema|listMatches|
|Normalized Schema|srcDevice_hostname|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|user_username|


