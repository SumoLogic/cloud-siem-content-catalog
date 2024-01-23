# [Rules](README.md): Active Directory Domain Enumeration

## Description
Potentially detects an attacker attempting to enumerate active users on the network. Attacks will use enumeration tools such as Bloodhound that will quickly query the domain controller by submitting multiple Kerberos ticket requests with forged device names to gather user and group information for those devices.

## Additional Details
|Detail|Value|
|----|----|
|Type|Threshold|
|Category|Credential Access|
|Apply Risk to Entities|device_hostname, device_ip, user_username|
|Signal Name|Active Directory Domain Enumeration|
|Summary Expression|Potential Active Directory enumeration attempt by user: {{user_username}} on host: {{device_hostname}}|
|Threshold Count|50|
|Threshold Window|5m|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0006, _mitreAttackTactic:TA0007, _mitreAttackTechnique:T1087, _mitreAttackTechnique:T1482, _mitreAttackTechnique:T1087.001, _mitreAttackTechnique:T1087.002|
## Vendors and Products
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Direct from Record|fields['insertionstrings_f09']|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|success|
|Normalized Schema|user_username|


