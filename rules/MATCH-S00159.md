# [Rules](README.md): Windows - Permissions Group Discovery

## Description
Microsoft’s Net.exe can be used for multiple Discovery tactics, including Password Policy, Permissions, Account and Domain Trust Discovery. This detection identifies the use net.exe related commands on a system related to these discovery tactics. It is recommended to investigate the host and user to determine if this is authorized admin activity or needs further inspection.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Discovery|
|Apply Risk to Entities|device_hostname, device_ip, user_username|
|Signal Name|Detected Discovery using net.exe on host|
|Summary Expression|Detected permission group discovery using net.exe on host: {{device_hostname}}|
|Score/Severity|Static: 1|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0007, _mitreAttackTechnique:T1069, _mitreAttackTechnique:T1069.001, _mitreAttackTechnique:T1069.002, _mitreAttackTechnique:T1201|
## Vendors and Products
- [CrowdStrike - FDR](../products/569a3a44-c29f-492e-bcf4-5dc04e2ab0f3.md)
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|baseImage|
|Normalized Schema|commandLine|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|listMatches|
|Normalized Schema|user_username|


