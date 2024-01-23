# [Rules](README.md): Possible TOR Connection

## Description
The subject and issuer of the SSL certificate match the pattern for certificates used by TOR connections.

## Additional Details
|Detail|Value|
|----|----|
|Type|Threshold|
|Category|Exfiltration|
|Apply Risk to Entities|device_hostname, device_ip, srcDevice_hostname, srcDevice_ip, user_username|
|Signal Name|Possible TOR Connection|
|Summary Expression|Potential TOR connection from IP: {{srcDevice_ip}}|
|Threshold Count|3|
|Threshold Window|5m|
|Score/Severity|Static: 5|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0010, _mitreAttackTactic:TA0011, _mitreAttackTechnique:T1090, _mitreAttackTechnique:T1090.002, _mitreAttackTechnique:T1573, _mitreAttackTechnique:T1573.001|
## Vendors and Products
- [Bro - Bro](../products/37C866BF-72E1-470A-9072-EDB908F56951.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|bro_ssl_issuer|
|Normalized Schema|bro_ssl_subject|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|srcDevice_hostname|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|user_username|


