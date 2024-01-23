# [Rules](README.md): Rogue DHCP Server - Cisco

## Description
Observes for Cisco events indicating the presence of a rogue DHCP server

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Collection|
|Apply Risk to Entities|device_hostname, srcDevice_ip, srcDevice_hostname, dstDevice_hostname, srcDevice_mac|
|Signal Name|Rogue DHCP Server - Cisco|
|Summary Expression|Rogue DHCP server detected on IP: {{device_ip}}|
|Score/Severity|Static: 2|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0006, _mitreAttackTactic:TA0009, _mitreAttackTactic:TA0001, _mitreAttackTechnique:T1557, _mitreAttackTechnique:T1557.002, _mitreAttackTechnique:T1200|
## Vendors and Products
- [Cisco Systems - Router and Switch IOS](../products/1abefd5b-ec3d-49c1-8a54-7e6363d52db0.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|device_hostname|
|Normalized Schema|dstDevice_hostname|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_vendor|
|Normalized Schema|srcDevice_hostname|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|srcDevice_mac|


