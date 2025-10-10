# [Rules](README.md): Outbound TFTP Traffic

## Description
TFTP is rarely used externally and has been observed as a means to deliver malicious code from the outside.

## Additional Details
|Detail|Value|
|----|----|
|Type|Match|
|Category|Execution|
|Apply Risk to Entities|device_ip, user_username, device_hostname, srcDevice_ip|
|Signal Name|Outbound TFTP Traffic|
|Summary Expression|Outbound TFTP traffic from IP: {{srcDevice_ip}} to IP: {{dstDevice_ip}}|
|Score/Severity|Static: 5|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0002, _mitreAttackTactic:TA0011, _mitreAttackTechnique:T1071, _mitreAttackTechnique:T1071.002|
## Vendors and Products
- [Bro - Bro](../products/37C866BF-72E1-470A-9072-EDB908F56951.md)
- [Cisco Systems - ASA](../products/be4f7473-fe69-4311-8859-3561900060bf.md)
- [Cisco Systems - Firepower](../products/da9e05a5-3fd3-46a7-a107-ae03c01e3f5a.md)
- [Cisco Systems - Meraki](../products/724c9add-8cd9-4013-b9e1-a907b96da426.md)
- [Dell - Firewall](../products/b1639f7f-4c11-4d29-ab69-368cf0e05e25.md)
- [Palo Alto Networks - Next Generation Firewall](../products/46f5fa2c-1a62-4692-82ad-ed87800a0adb.md)
- [Palo Alto Networks - Prisma Cloud](../products/343b9323-d279-40d9-946f-809242e5cf98.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|dstDevice_ip_isInternal|
|Normalized Schema|dstPort|
|Normalized Schema|ipProtocol|
|Normalized Schema|listMatches|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|srcDevice_ip_isInternal|
|Normalized Schema|user_username|


