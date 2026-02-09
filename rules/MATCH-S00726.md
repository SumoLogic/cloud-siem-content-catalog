# [Rules](README.md): macOS Kernel Extension Load

## Description
Kernel Extensions in macOS can be used by adversaries to execute malicious code with root privileges.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Persistence|
|Apply Risk to Entities|device_hostname, device_ip, user_username|
|Signal Name|macOS Kernel Extension Load|
|Summary Expression|Observed kextload command on host: {{device_hostname}}|
|Score/Severity|Static: 2|
|Enabled by Default|True|
|Prototype|True|
|Tags|_mitreAttackTechnique:T1547, _mitreAttackTechnique:T1547.006, _mitreAttackTactic:TA0003|
## Vendors and Products
- [CrowdStrike - FDR](../products/569a3a44-c29f-492e-bcf4-5dc04e2ab0f3.md)
- [Cylance - Protect](../products/60829f4a-7acb-47d1-ad23-8424fcf83dcb.md)
- [Jamf - Jamf](../products/5c2cc0de-ca31-4ef0-bcfa-133fc8b387ad.md)
- [Microsoft - Azure](../products/a1225af5-e778-4068-a9a2-47da93d1ff24.md)
- [Microsoft - Defender Advanced Hunting](../products/3382523e-2072-41bd-b50b-6b148957d0b0.md)
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)
- [Osquery - Osquery](../products/93e2d3d-fab1-4d61-845f-49bc1ae5bed9.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|commandLine|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|user_username|


