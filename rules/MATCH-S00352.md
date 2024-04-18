# [Rules](README.md): MSHTA Suspicious Execution

## Description
Detection for mshta.exe suspicious execution patterns sometimes involving file polyglotism.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Defense Evasion|
|Apply Risk to Entities|device_hostname, device_ip, user_username|
|Signal Name|MSHTA Suspicious Execution|
|Summary Expression|Suspicious command: {{commandLine}} executed on host: {{device_hostname}}|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0005, _mitreAttackTechnique:T1140, _mitreAttackTechnique:T1218, _mitreAttackTechnique:T1218.005|
## Vendors and Products
- [CrowdStrike - FDR](../products/569a3a44-c29f-492e-bcf4-5dc04e2ab0f3.md)
- [Cylance - Protect](../products/60829f4a-7acb-47d1-ad23-8424fcf83dcb.md)
- [Microsoft - Azure](../products/a1225af5-e778-4068-a9a2-47da93d1ff24.md)
- [Microsoft - Office 365](../products/d3ed003d-5ddd-4c7a-bea5-63eae6311833.md)
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)
- [Tanium - Tanium Core](../products/5b49e894-92e8-45ad-8575-fe78b4f2e31b.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|baseImage|
|Normalized Schema|commandLine|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|user_username|


