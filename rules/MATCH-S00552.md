# [Rules](README.md): Windows Connhost Started Forcefully

## Description
The rule looks for the Console Window Host process (connhost.exe) executed using the force flag -ForceV1. This is not regular behavior in the Windows OS and is often seen executed by the Ryuk Ransomware. The rule is disabled by default as this may be common in some environments.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Execution|
|Apply Risk to Entities|device_hostname, user_username, device_ip|
|Signal Name|Windows Connhost Started Forcefully|
|Summary Expression|Windows Connhost has been started forcefully on host: {{device_hostname}}|
|Score/Severity|Static: 1|
|Enabled by Default|False|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0002, _mitreAttackTechnique:T1059, _mitreAttackTechnique:T1059.003|
## Vendors and Products
- [CrowdStrike - FDR](../products/569a3a44-c29f-492e-bcf4-5dc04e2ab0f3.md)
- [Cylance - Protect](../products/60829f4a-7acb-47d1-ad23-8424fcf83dcb.md)
- [Microsoft - Azure](../products/a1225af5-e778-4068-a9a2-47da93d1ff24.md)
- [Microsoft - Defender Advanced Hunting](../products/3382523e-2072-41bd-b50b-6b148957d0b0.md)
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|commandLine|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|user_username|


