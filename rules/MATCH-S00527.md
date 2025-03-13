# [Rules](README.md): Email Files Written Outside Of The Outlook Directory

## Description
The rule detects email files created outside the normal Outlook directory.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Defense Evasion|
|Apply Risk to Entities|device_hostname, device_ip, user_username|
|Signal Name|Email Files Written Outside Of The Outlook Directory|
|Summary Expression|Email file: {{file_basename}} written outside Outlook directory on host {{device_hostname}}|
|Score/Severity|Static: 4|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0005, _mitreAttackTechnique:T1036, _mitreAttackTechnique:T1036.005, _mitreAttackTechnique:T1036.004|
## Vendors and Products
- [Cisco Systems - ASA](../products/be4f7473-fe69-4311-8859-3561900060bf.md)
- [Code42 - Incydr](../products/cc523ad6-7193-4de5-a254-d0243fca63f3.md)
- [Digital Guardian - ARC](../products/975d678e-eb46-4155-9427-0fa307971fcd.md)
- [Egnyte - DLP](../products/114420df-d10c-4e88-92e9-0d95102c1a3d.md)
- [Google - G Suite](../products/e73cd65a-7a4b-4ce9-9d73-e5d9c824c214.md)
- [Microsoft - Azure](../products/a1225af5-e778-4068-a9a2-47da93d1ff24.md)
- [Microsoft - Defender Advanced Hunting](../products/3382523e-2072-41bd-b50b-6b148957d0b0.md)
- [Microsoft - Graph Security API](../products/ef42eb74-7444-4fee-b231-b4eb1e7c9660.md)
- [Microsoft - Office 365](../products/d3ed003d-5ddd-4c7a-bea5-63eae6311833.md)
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)
- [Netskope - Security Cloud](../products/B3582ED2-1A0C-452D-9802-97433D143486.md)
- [Zscaler - Nanolog Streaming Service](../products/6299d728-14f7-455e-85c5-ea8ec65a654a.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|baseImage|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|file_basename|
|Normalized Schema|file_path|
|Normalized Schema|lower|
|Normalized Schema|user_username|


