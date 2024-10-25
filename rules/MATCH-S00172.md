# [Rules](README.md): Windows - WiFi Credential Harvesting with netsh

## Description
Harvesting of Wifi Credentials Using netsh.exe

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Discovery|
|Apply Risk to Entities|device_hostname, device_ip, user_username|
|Signal Name|WiFi Credential Harvesting with netsh|
|Summary Expression|Detected WiFi credential harvesting using netsh on host: {{device_hostname}}|
|Score/Severity|Static: 1|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0006, _mitreAttackTactic:TA0007, _mitreAttackTechnique:T1040|
## Vendors and Products
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|commandLine|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|listMatches|
|Normalized Schema|parentBaseImage|
|Normalized Schema|user_username|


