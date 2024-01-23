# [Rules](README.md): Fake Windows Processes

## Description
Observes for known Windows processes being executed outside of normal directories (System32 and SysWOW64). This would indicate process masquerading.

Note that this rule requires creating a match list 'known_windows_processes' containing known OK Windows processes that would not normally be executed outside of System32 or SysWOW64.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Defense Evasion|
|Apply Risk to Entities|device_hostname, device_ip, user_username|
|Signal Name|Fake Windows Processes|
|Summary Expression|Potential fake Windows process: {{baseImage}} on host: {{device_hostname}}|
|Score/Severity|Static: 3|
|Enabled by Default|False|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0005, _mitreAttackTechnique:T1036, _mitreAttackTechnique:T1036.003, _mitreAttackTechnique:T1036.004, _mitreAttackTechnique:T1036.005|
## Vendors and Products
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|listMatches|
|Normalized Schema|user_username|


