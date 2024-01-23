# [Rules](README.md): Self-signed Certificates

## Description
A server responded on a SSL or TLS service using a self-signed certificate.

## Additional Details
|Detail|Value|
|----|----|
|Type|Match|
|Category|Exfiltration|
|Apply Risk to Entities|srcDevice_ip|
|Signal Name|Self-signed Certificates|
|Summary Expression|Server IP: {{srcDevice_ip}} with SSL or TLS service responded with self-signed certificate|
|Score/Severity|Static: 1|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0005, _mitreAttackTactic:TA0010, _mitreAttackTechnique:T1553, _mitreAttackTechnique:T1553.002|
## Vendors and Products
- [Bro - Bro](../products/37C866BF-72E1-470A-9072-EDB908F56951.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|dstDevice_ip_isInternal|
|Direct from Record|fields['issuer']|
|Direct from Record|fields['subject']|
|Normalized Schema|listMatches|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_vendor|
|Normalized Schema|srcDevice_ip|


