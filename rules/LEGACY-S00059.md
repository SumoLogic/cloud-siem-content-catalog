# [Rules](README.md): Port Scan - External

## Description
External port scan. A host external to the monitored network was detected as showing behavior consistent with a scan for a port on multiple destination addresses in a short time.

## Additional Details
|Detail|Value|
|----|----|
|Type|Match|
|Category|Discovery|
|Apply Risk to Entities|device_ip, user_username, device_hostname, srcDevice_ip|
|Signal Name|Port Scan - External|
|Summary Expression|External port scan from IP:: {{srcDevice_ip}}|
|Score/Severity|Static: 2|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0043, _mitreAttackTechnique:T1595, _mitreAttackTechnique:T1046, _mitreAttackTechnique:T1595.001|
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


