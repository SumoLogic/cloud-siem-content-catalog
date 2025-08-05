# [Rules](README.md): Unload Sysmon Filter Driver

## Description
Attackers often disable security tools to avoid detection. This rule looks for the usage of process fltMC.exe to unload a Sysmon Driver that will stop sysmon from collecting the data.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Defense Evasion|
|Apply Risk to Entities|user_username, device_ip, device_hostname|
|Signal Name|Unload Sysmon Filter Driver|
|Summary Expression|Attempt to unload Sysmon filter driver on host: {{device_hostname}}|
|Score/Severity|Static: 5|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0005, _mitreAttackTechnique:T1562, _mitreAttackTechnique:T1562.001, _mitreAttackTechnique:T1562.002, _mitreAttackTechnique:T1562.003, _mitreAttackTechnique:T1562.006|
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
|Normalized Schema|user_username|


