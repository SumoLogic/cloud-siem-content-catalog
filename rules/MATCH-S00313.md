# [Rules](README.md): Unauthorized External Device Installation

## Description
Detects a removable media device attached to a host. External media can be used to exfiltrate sensitive data and is also a common source of infections, so some organizations block their use. Attempts to use these devices could indicate the intent for malicious activity. Customer should populate a list of devices that should not have external media installed on them.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Exfiltration|
|Apply Risk to Entities|device_hostname, device_ip, user_username|
|Signal Name|Unauthorized External Device Installation|
|Summary Expression|Unauthorized external device installation on host: {{device_hostname}}|
|Score/Severity|Static: 5|
|Enabled by Default|False|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0009, _mitreAttackTactic:TA0010, _mitreAttackTactic:TA0011, _mitreAttackTechnique:T1025, _mitreAttackTechnique:T1052, _mitreAttackTechnique:T1052.001, _mitreAttackTechnique:T1092|
## Vendors and Products
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|listMatches|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|user_username|


