# [Rules](README.md): Noncompliant Protocol Tunnel Over Common Service Port

## Description
Tools or malware may be configured to send communications over a network by using a common service port to carry unrelated traffic. This is often done to bypass security controls or to obfuscate malicious traffic by mimicking a legitimate service. For example, this is often done with UDP based VPN tunnels connecting over port 53. https://attack.mitre.org/techniques/T1043/ describes the use of this technique by attackers.

## Additional Details
|Detail|Value|
|----|----|
|Type|Match|
|Category|Command and Control|
|Apply Risk to Entities|device_ip, user_username, device_hostname, srcDevice_ip|
|Signal Name|Noncompliant Protocol Tunnel Over Common Service Port|
|Summary Expression|Noncompliant protocol tunnel to port: {{dstPort}} from IP: {srcDevice_ip}}|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0011, _mitreAttackTechnique:T1071, _mitreAttackTechnique:T1071.004|
## Vendors and Products
- [Bro - Bro](../products/37C866BF-72E1-470A-9072-EDB908F56951.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|bro_flow_duration|
|Normalized Schema|bro_flow_service|
|Normalized Schema|bytesIn|
|Normalized Schema|bytesOut|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|dstDevice_ip_isInternal|
|Normalized Schema|dstPort|
|Normalized Schema|ipProtocol|
|Normalized Schema|listMatches|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_product|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|srcDevice_ip_isInternal|
|Normalized Schema|user_username|


