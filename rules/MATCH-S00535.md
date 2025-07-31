# [Rules](README.md): Golden SAML Indicator : Certificate Export

## Description
Observes for multiple methods of certificate export which may indicate that an attacker is attempting to bypass multifactor authentication using a stolen certificate.

This rule utilizes indicators from Windows command line auditing, PowerShell auditing, and Sysmon named pipe connections.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Credential Access|
|Apply Risk to Entities|device_hostname, user_username|
|Signal Name|Golden SAML Detection : Certificate Export|
|Summary Expression|Certificate export observed on host: {{device_hostname}} by user: {{user_username}}|
|Score/Severity|Static: 4|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0011, _mitreAttackTactic:TA0004, _mitreAttackTechnique:T1105, _mitreAttackTechnique:T1548, _mitreAttackTechnique:T1548.002|
## Vendors and Products
- [CrowdStrike - FDR](../products/569a3a44-c29f-492e-bcf4-5dc04e2ab0f3.md)
- [Microsoft - Azure](../products/a1225af5-e778-4068-a9a2-47da93d1ff24.md)
- [Microsoft - Defender Advanced Hunting](../products/3382523e-2072-41bd-b50b-6b148957d0b0.md)
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|baseImage|
|Normalized Schema|commandLine|
|Normalized Schema|device_hostname|
|Normalized Schema|user_username|


