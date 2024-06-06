# [Rules](README.md): Attempted Credential Dump From Registry Via Reg.Exe

## Description
Monitors for use of reg.exe with parameters indicating the attempted export of hashed credentials.

Audit Object Access (success & failure) must be enabled for this rule to function.

Monitoring of the following registry keys is necessary:
HKLM\Security
HKLM\Security\Cache
HKLM\System
HKLM\Security\Policy\Secrets
HKLM\Sam

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Credential Access|
|Apply Risk to Entities|device_hostname, device_ip, user_username|
|Signal Name|Attempted Credential Dump From Registry Via Reg.exe|
|Summary Expression|Attempt to export credentials detected on host: {{device_hostname}} by user: {{user_username}}|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0005, _mitreAttackTactic:TA0008, _mitreAttackTactic:TA0006, _mitreAttackTechnique:T1550, _mitreAttackTechnique:T1003, _mitreAttackTechnique:T1550.002|
## Vendors and Products
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Direct from Record|fields['EventData.ProcessName']|
|Normalized Schema|file_path|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|user_username|


