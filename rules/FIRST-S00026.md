# [Rules](README.md): First Seen Anonymous Logon Change Activity to Domain Controller

## Description
Attackers can attempt to hijack enterprise servers exploiting Netlogon cryptographic weaknesses. The vulnerability allows an attacker to set a password for the computer account of an Active Directory Domain Controller, which can then be abused to pull credentials from the Domain Controller. This rule detects fist seen anonymous user attempt a change on a domain controller computer account.

## Additional Details
|Detail|Value|
|----|----|
|Type|First Seen|
|Category|Lateral Movement|
|Apply Risk to Entities|device_hostname|
|Signal Name|First Seen Anonymous Logon Change Activity to Domain Controller host|
|Summary Expression|Detected anonymous logon activity on domain controller host: {{device_hostname}}|
|Retention Window|7776000000|
|Baseline Window|3024000000|
|Baseline Type|GLOBAL|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0006, _mitreAttackTechnique:T1003, _mitreAttackTechnique:T1003.005|
## Vendors and Products
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|device_hostname|
|Normalized Schema|listMatches|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|user_username|


