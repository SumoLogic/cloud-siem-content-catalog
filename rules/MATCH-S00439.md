# [Rules](README.md): Psr.exe Capture Screenshots

## Description
The psr.exe captures desktop screenshots and saves them on the local machine.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Collection|
|Apply Risk to Entities|device_hostname, device_ip, user_username|
|Signal Name|Psr.exe Capture Screenshots|
|Summary Expression|Process: {{baseImage}} executed on host: {{device_hostname}} with command: {{commandLine}}|
|Score/Severity|Static: 4|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0009, _mitreAttackTechnique:T1113|
## Vendors and Products
- [Microsoft - Azure](../products/a1225af5-e778-4068-a9a2-47da93d1ff24.md)
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)
- [Tanium - Tanium Core](../products/5b49e894-92e8-45ad-8575-fe78b4f2e31b.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|baseImage|
|Normalized Schema|commandLine|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|user_username|


