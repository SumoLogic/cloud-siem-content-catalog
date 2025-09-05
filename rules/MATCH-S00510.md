# [Rules](README.md): Attempt to Add Certificate to Store

## Description
Observes for attempts to add a certificate to the untrusted store

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Defense Evasion|
|Apply Risk to Entities|device_hostname, user_username|
|Signal Name|Attempt to Add Certificate to Store|
|Summary Expression|Attempt to add certificate to store on host: {{device_hostname}} by user: {{user_username}}|
|Score/Severity|Static: 0|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0005, _mitreAttackTechnique:T1553, _mitreAttackTechnique:T1553.002, _mitreAttackTechnique:T1553.004|
## Vendors and Products
- [CrowdStrike - FDR](../products/569a3a44-c29f-492e-bcf4-5dc04e2ab0f3.md)
- [Microsoft - Azure](../products/a1225af5-e778-4068-a9a2-47da93d1ff24.md)
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|baseImage|
|Normalized Schema|commandLine|
|Normalized Schema|device_hostname|
|Normalized Schema|user_username|


