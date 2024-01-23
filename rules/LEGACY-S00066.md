# [Rules](README.md): PowerShell Remote Administration

## Description
Remote Administration from Powershell is logged by default in the admin$temp  folder.  These commands should only be associated with IP addresses that are expected to carry out remote administration tasks.

## Additional Details
|Detail|Value|
|----|----|
|Type|Match|
|Category|Lateral Movement|
|Apply Risk to Entities|device_hostname, device_ip, srcDevice_hostname, srcDevice_ip, user_username|
|Signal Name|PowerShell Remote Administration|
|Summary Expression|Remote Powershell administration detected from IP: {{srcDevice_ip}}|
|Score/Severity|Static: 4|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0008, _mitreAttackTechnique:T1021, _mitreAttackTechnique:T1021.006, _mitreAttackTechnique:T1059, _mitreAttackTechnique:T1059.001, _mitreAttackTechnique:T1059.003|
## Vendors and Products
- [Bro - Bro](../products/37C866BF-72E1-470A-9072-EDB908F56951.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|file_basename|
|Normalized Schema|file_path|
|Normalized Schema|listMatches|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_product|
|Normalized Schema|srcDevice_hostname|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|user_username|


