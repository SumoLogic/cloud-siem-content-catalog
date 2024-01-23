# [Rules](README.md): Windows Firewall Rule Modified

## Description
Observes for modifications to Windows Firewall rules. An attacker may modify firewall rules to obfuscate activities via blocks, or to allow certain activity through the firewall.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Defense Evasion|
|Apply Risk to Entities|device_hostname, user_username|
|Signal Name|Windows Firewall Rule Modified|
|Summary Expression|Windows Firewall rule modified on host: {{device_hostname}}|
|Score/Severity|Static: 1|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0005, _mitreAttackTechnique:T1562, _mitreAttackTechnique:T1562.001, _mitreAttackTechnique:T1562.004|
## Vendors and Products
- [Microsoft - Windows Firewall Management](../products/e91e068a-fe7e-45d4-98c6-1cc1e3d4d99f.md)
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|device_hostname|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|user_username|


