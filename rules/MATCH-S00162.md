# [Rules](README.md): Windows - Network trace capture using netsh.exe

## Description
Detects capture of a network trace via the netsh.exe trace functionality

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Discovery|
|Apply Risk to Entities|device_hostname, device_ip, user_username|
|Signal Name|netsh.exe is being used to capture a network trace.|
|Summary Expression|Detected network trace using netsh on host: {{device_hostname}}|
|Score/Severity|Static: 1|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0006, _mitreAttackTactic:TA0007, _mitreAttackTechnique:T1016, _mitreAttackTechnique:T1016.001, _mitreAttackTechnique:T1040|
## Vendors and Products
- [CrowdStrike - FDR](../products/569a3a44-c29f-492e-bcf4-5dc04e2ab0f3.md)
- [Microsoft - Azure](../products/a1225af5-e778-4068-a9a2-47da93d1ff24.md)
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)
- [VMware - Carbon Black Cloud](../products/f9cea291-9030-4e41-9836-6dd9274d6df4.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|commandLine|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|listMatches|
|Normalized Schema|parentBaseImage|
|Normalized Schema|user_username|


