# [Rules](README.md): First Seen Get-ADDefaultDomainPasswordPolicy

## Description
The first observed execution of the PowerShell CMDLet Get-ADDefaultDomainPasswordPolicy on this host, this CMDLet can be used in the discovery of Windows Domain Password Policies by threat actors. Investigating the host and active users for additional activity around the time of execution is recommended.

## Additional Details
|Detail|Value|
|----|----|
|Type|First Seen|
|Category|Discovery|
|Apply Risk to Entities|device_hostname, device_ip|
|Signal Name|First Seen Get-ADDefaultDomainPasswordPolicy on Host:{{device_hostname}}|
|Summary Expression|The PowerShell CMDLet Get-ADDefaultDomainPasswordPolicy has been observed being executed on this host.|
|Retention Window|7776000000|
|Baseline Window|1209600000|
|Baseline Type|GLOBAL|
|Score/Severity|Static: 2|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0007, _mitreAttackTechnique:T1201|
## Vendors and Products
- [CrowdStrike - FDR](../products/569a3a44-c29f-492e-bcf4-5dc04e2ab0f3.md)
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|commandLine|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|


