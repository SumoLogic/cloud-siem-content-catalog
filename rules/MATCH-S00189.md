# [Rules](README.md): Windows Admin User Remote Logon

## Description
Detects remote logins by Administrative users. Administrative users are identified using your local naming convention. Because each environment controls their user naming convention, this rule's expression must first be tailored around your environment and enabled.  Adjust the section that reads:  "LIKE '%admin%'" to your environment's administrator naming convention.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Lateral Movement|
|Apply Risk to Entities|device_hostname, device_ip, user_username|
|Signal Name|Windows Admin User Remote Logon|
|Summary Expression|Remote logon by administrative user: {{user_username}} on host: {{device_hostname}}|
|Score/Severity|Static: 1|
|Enabled by Default|False|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0008, _mitreAttackTechnique:T1021, _mitreAttackTechnique:T1021.001, _mitreAttackTechnique:T1021.006|
## Vendors and Products
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Direct from Record|fields['EventData.AuthenticationPackageName']|
|Normalized Schema|logonType|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|objectType|
|Normalized Schema|user_username|


