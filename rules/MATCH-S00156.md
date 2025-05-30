# [Rules](README.md): New Suspicious cmd.exe / regedit.exe / powershell.exe Service Launch

## Description
The Service Control Manager, or services.exe, has no legitimate reason to launch commands like cmd.exe, powershell.exe, or regedit.exe. Incidentally, a common way for malware to masquerade as something legitimate is to call itself service.exe.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Persistence|
|Apply Risk to Entities|device_hostname, device_ip, user_username|
|Signal Name|New Suspicious {{baseImage}}  Service Launch|
|Summary Expression|Process: services.exe launched child process: {{baseImage}}|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0002, _mitreAttackTactic:TA0003, _mitreAttackTechnique:T1059, _mitreAttackTechnique:T1059.001, _mitreAttackTechnique:T1059.003|
## Vendors and Products
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|baseImage|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|parentBaseImage|
|Normalized Schema|user_username|


