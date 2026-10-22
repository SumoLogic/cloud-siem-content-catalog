# [Rules](README.md): Suspicious PowerShell Window Discovery Cmdlet execution

## Description
Detects the use of PowerShell for Applicaiton Window Discovery to identify open application windows to gather information on running programs, collect potential data, and discover security tooling. Investigation into the host and user to identify the process executing the PowerShell function. Reference: https://www.ired.team/offensive-security/enumeration-and-discovery/t1010-application-window-discovery

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Discovery|
|Apply Risk to Entities|device_hostname|
|Signal Name|Suspicious PowerShell Window Discovery Cmdlet execution on {{device_hostname}}|
|Summary Expression|PowerShell Window Discovery Cmdlet execution to obtain open applications using mainWindowTitle on {{device_hostname}}|
|Score/Severity|Static: 2|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0007, _mitreAttackTechnique:T1010|
## Vendors and Products
- [CrowdStrike - FDR](../products/569a3a44-c29f-492e-bcf4-5dc04e2ab0f3.md)
- [CrowdStrike - Falcon](../products/840c72e0-4e47-41e7-9b93-31f55d12f07d.md)
- [Microsoft - Azure](../products/a1225af5-e778-4068-a9a2-47da93d1ff24.md)
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)
- [Trend Micro - Vision One](../products/72a5ddec-abb9-41ff-a2da-6a58beff980c.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|commandLine|
|Normalized Schema|device_hostname|


