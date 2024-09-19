# [Rules](README.md): Volume Shadow Copy Service Stopped

## Description
Detects the Volume Shadow Copy service being stopped using net stop. This activity is commonly seen in wiper malware and ransomware attacks.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Impact|
|Apply Risk to Entities|device_hostname, user_username, device_ip|
|Signal Name|Volume Shadow Copy Service Stopped|
|Summary Expression|The Volume Shadow Copy Service has been stopped on host: {{device_hostname}}|
|Score/Severity|Static: 5|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0040, _mitreAttackTechnique:T1489, _mitreAttackTechnique:T1490|
## Vendors and Products
- [CrowdStrike - FDR](../products/569a3a44-c29f-492e-bcf4-5dc04e2ab0f3.md)
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|commandLine|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|user_username|


