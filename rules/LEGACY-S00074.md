# [Rules](README.md): SMB Internal to External traffic

## Description
SMB/CIFS is a workgroup protocol for file sharing intended to be used among trusted systems on an internal LAN. A number of risks are associated with internal systems connecting to untrusted external SMB servers, including exploit delivery, credential harvesting, and data exfiltration. SMB access should be limited to the enterprise network to prevent participation in unknown SMB related attacks. Limited exceptions may exist, such as file server access over extranet connections.

## Additional Details
|Detail|Value|
|----|----|
|Type|Match|
|Category|Lateral Movement|
|Apply Risk to Entities|device_hostname, device_ip, srcDevice_hostname, srcDevice_ip, user_username|
|Signal Name|SMB Internal to External traffic|
|Summary Expression|Internal IP: {{srcDevice_ip}} connecting to external file share on IP: {{srcDevice_ip}}|
|Score/Severity|Static: 4|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0008, _mitreAttackTechnique:T1021, _mitreAttackTechnique:T1021.002|
## Vendors and Products
- [Bro - Bro](../products/37C866BF-72E1-470A-9072-EDB908F56951.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|dstDevice_ip_isInternal|
|Normalized Schema|listMatches|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_product|
|Normalized Schema|srcDevice_hostname|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|srcDevice_ip_isInternal|
|Normalized Schema|user_username|


