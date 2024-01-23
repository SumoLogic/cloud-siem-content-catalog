# [Rules](README.md): First Seen Access - SMB Share

## Description
Adversaries may access a networked system remotely using Server Message Block (SMB) to transfer files, and run transferred binaries through remote execution. Although not malicious on its own, this first-seen access to a DISK share over SMB can be an indicator of lateral movement.

## Additional Details
|Detail|Value|
|----|----|
|Type|Match|
|Category|Lateral Movement|
|Apply Risk to Entities|device_ip, user_username, device_hostname, srcDevice_ip|
|Signal Name|First Seen Access - SMB Share|
|Summary Expression|First time SMB share access from: {{srcDevice_ip}}|
|Score/Severity|Static: 1|
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
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_product|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|srcDevice_ip_isInternal|
|Normalized Schema|threat_name|
|Normalized Schema|user_username|


