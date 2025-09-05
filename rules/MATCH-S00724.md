# [Rules](README.md): Windows Update Agent DLL Changed

## Description
The Windows Update Agent executable, wuauclt.exe, can be abused by attackers to execute malicious code with elevated privileges by changing the DLL file loaded by the process. This technique is most commonly reported as part of phishing campaigns where the initial payload is a macro-enabled Microsoft Word document.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Defense Evasion|
|Apply Risk to Entities|user_username, device_hostname|
|Signal Name|Windows Update Agent DLL Changed|
|Summary Expression|User {{user_username}} ran a command on host {{device_hostname}} to modify the Windows Update Agent|
|Score/Severity|Static: 4|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTechnique:T1218.011, _mitreAttackTactic:TA0005, _mitreAttackTechnique:T1129|
## Vendors and Products
- [CrowdStrike - FDR](../products/569a3a44-c29f-492e-bcf4-5dc04e2ab0f3.md)
- [CrowdStrike - Falcon](../products/840c72e0-4e47-41e7-9b93-31f55d12f07d.md)
- [Microsoft - Azure](../products/a1225af5-e778-4068-a9a2-47da93d1ff24.md)
- [Microsoft - Defender Advanced Hunting](../products/3382523e-2072-41bd-b50b-6b148957d0b0.md)
- [Microsoft - Office 365](../products/d3ed003d-5ddd-4c7a-bea5-63eae6311833.md)
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|commandLine|
|Normalized Schema|device_hostname|
|Normalized Schema|user_username|


