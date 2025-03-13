# [Rules](README.md): Chromium Process Started With Debugging Port

## Description
Chromium (Microsoft Edge or Google Chrome) browsers can be started with a remote debugging port. Threat actors may then connect to this debugging port to enumerate browser information or steal session data including browser cookies.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Credential Access|
|Apply Risk to Entities|user_username, device_hostname|
|Signal Name|Chromium Process Started With Debugging Port|
|Summary Expression|The Chromium process {{baseImage}} was started via {{parentBaseImage}} with remote debugging enabled.|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0006, _mitreAttackTechnique:T1555.003, _mitreAttackTechnique:T1606.001, _mitreAttackTechnique:T1539|
## Vendors and Products
- [CrowdStrike - FDR](../products/569a3a44-c29f-492e-bcf4-5dc04e2ab0f3.md)
- [CrowdStrike - Falcon](../products/840c72e0-4e47-41e7-9b93-31f55d12f07d.md)
- [Microsoft - Azure](../products/a1225af5-e778-4068-a9a2-47da93d1ff24.md)
- [Microsoft - Defender Advanced Hunting](../products/3382523e-2072-41bd-b50b-6b148957d0b0.md)
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|device_hostname|
|Normalized Schema|user_username|


