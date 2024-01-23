# [Rules](README.md): Interactive Logon to Domain Controller

## Description
Detects an interactive login to a domain controller. Direct access in this manner is rarely necessary and should be closely audited given the potential impact of a compromised domain controller.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Persistence|
|Apply Risk to Entities|user_username, dstDevice_hostname, srcDevice_ip|
|Signal Name|Interactive Logon to Domain Controller|
|Summary Expression|Interactive logon on domain controller: {{device_hostname}} with account: {{user_username}}|
|Score/Severity|Static: 5|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0003, _mitreAttackTactic:TA0004, _mitreAttackTactic:TA0008, _mitreAttackTechnique:T1021.001|
## Vendors and Products
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|dstDevice_hostname|
|Normalized Schema|listMatches|
|Normalized Schema|logonType|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|user_username|


