# [Rules](README.md): PowerShell File Download

## Description
PowerShell scripts are commonly used as droppers, which will download additional tools onto a compromised host.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Execution|
|Apply Risk to Entities|device_hostname, device_ip, user_username|
|Signal Name|PowerShell File Download|
|Summary Expression|Powershell file download command executed on host: {{device_hostname}}|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0002, _mitreAttackTactic:TA0011, _mitreAttackTechnique:T1059, _mitreAttackTechnique:T1105, _mitreAttackTechnique:T1059.001, _mitreAttackTechnique:T1059.003|
## Vendors and Products
- [Bitdefender - GravityZone](../products/046b3623-69fe-409f-9e80-fd3ebef0654f.md)
- [CrowdStrike - FDR](../products/569a3a44-c29f-492e-bcf4-5dc04e2ab0f3.md)
- [CrowdStrike - Falcon](../products/840c72e0-4e47-41e7-9b93-31f55d12f07d.md)
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)
- [VMware - Carbon Black Cloud](../products/f9cea291-9030-4e41-9836-6dd9274d6df4.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|baseImage|
|Normalized Schema|commandLine|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|user_username|


