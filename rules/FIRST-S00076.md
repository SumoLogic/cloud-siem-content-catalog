# [Rules](README.md): First Seen Net Command Use on Host

## Description
Microsoft’s Net.exe can be used for multiple Discovery tactics, including Password Policy, Permissions, Account and Domain Trust Discovery. This detection identifies the first observance of a Net related command on a system related to these discovery tactics. It is recommended to investigate the host and user to determine if this is authorized admin activity or needs further inspection.

## Additional Details
|Detail|Value|
|----|----|
|Type|First Seen|
|Category|Discovery|
|Apply Risk to Entities|device_hostname, device_ip, user_username|
|Signal Name|First Seen net command use on host: {{device_hostname}}|
|Summary Expression|First observance of net command use on this Host: {{device_hostname}} by the account: {{user_username}}|
|Retention Window|7776000000|
|Baseline Window|2592000000|
|Baseline Type|GLOBAL|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0007, _mitreAttackTechnique:T1201, _mitreAttackTactic:TA0006, _mitreAttackTechnique:T1087, _mitreAttackTechnique:T1482, _mitreAttackTechnique:T1087.001, _mitreAttackTechnique:T1087.002|
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


