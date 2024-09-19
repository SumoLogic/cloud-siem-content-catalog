# [Rules](README.md): MacOS System Integrity Protection Disabled

## Description
The System Integrity Protection (SIP) feature of MacOS helps to prevent the execution of unauthorized code and disabling this feature can be an indicator of a malicious actor attempting to bypass default security features. Tuning for this rule may be necessary if software developers in the organization use MacOS and need to disable SIP to run their code.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Defense Evasion|
|Apply Risk to Entities|device_hostname, device_ip, user_username|
|Signal Name|MacOS System Integrity Protection Disabled|
|Summary Expression|User: {{user_username}} disabled System Integrity Protecion on host: {{device_hostname}}|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0005, _mitreAttackTechnique:T1553.006|
## Vendors and Products
- [CrowdStrike - FDR](../products/569a3a44-c29f-492e-bcf4-5dc04e2ab0f3.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|commandLine|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|user_username|


