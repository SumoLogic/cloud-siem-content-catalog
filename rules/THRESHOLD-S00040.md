# [Rules](README.md): Possible DNS over TLS (DoT) Activity

## Description
This rule detects attempted or successful connections to the standard service port for DoT services. DNS over TLS (RFC 7858, DoT) is a name resolution service that allows clients to resolve DNS records over encrypted and validated connections. DoT operates over standards compliant TLS and is specified to operate over port 853/tcp. In some environments this may be abused as a method to bypass security and policy controls. Some malicious actors leverage DoT to tunnel DNS traffic over TLS, and research has demonstrated the ability to carry out other DNS related abuse such as malware C2 over DoT as well.

## Additional Details
|Detail|Value|
|----|----|
|Type|Threshold|
|Category|Defense Evasion|
|Apply Risk to Entities|device_hostname, device_ip, srcDevice_hostname, srcDevice_ip, user_username|
|Signal Name|Possible DNS over TLS (DoT) Activity|
|Summary Expression|Possible DNS over TLS from source IP: {{srcDevice_ip}}|
|Threshold Count|1|
|Threshold Window|5m|
|Score/Severity|Static: 1|
|Enabled by Default|False|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0005, _mitreAttackTactic:TA0011, _mitreAttackTechnique:T1573, _mitreAttackTechnique:T1573.001, _mitreAttackTechnique:T1573.002|
## Vendors and Products
- [Bro - Bro](../products/37C866BF-72E1-470A-9072-EDB908F56951.md)
- [Cisco Systems - Firepower](../products/da9e05a5-3fd3-46a7-a107-ae03c01e3f5a.md)
- [Cisco Systems - Meraki](../products/724c9add-8cd9-4013-b9e1-a907b96da426.md)
- [Dell - Firewall](../products/b1639f7f-4c11-4d29-ab69-368cf0e05e25.md)
- [Palo Alto Networks - Next Generation Firewall](../products/46f5fa2c-1a62-4692-82ad-ed87800a0adb.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|dstDevice_ip_isInternal|
|Normalized Schema|dstPort|
|Normalized Schema|ipProtocol|
|Normalized Schema|listMatches|
|Normalized Schema|srcDevice_hostname|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|srcDevice_ip_isInternal|
|Normalized Schema|user_username|


