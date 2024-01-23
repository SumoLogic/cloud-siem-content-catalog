# [Rules](README.md): Windows - Suspicious Anonymous Logon Activity - Zerologon Behavior(CVE-2020-1472)

## Description
CVE-2020-1472 can be exploited by attackers to hijack enterprise servers due to Netlogon cryptographic weaknesses. The vulnerability allows an attacker to set a password for the computer account of an Active Directory Domain Controller, which can then be abused to pull credentials from the Domain Controller. This rule detects the domain controller computer account being changed after a successful anonymous login occurred.

## Additional Details
|Detail|Value|
|----|----|
|Type|Chain|
|Category|Lateral Movement|
|Apply Risk to Entities|user_username, device_hostname, device_ip, srcDevice_hostname, srcDevice_ip, dstDevice_hostname, dstDevice_ip|
|Signal Name|Windows - Suspicious Anonymous Logon Activity - Zerologon Behavior(CVE-2020-1472)|
|Summary Expression|Detected anonymous logon activity on host: {{device_hostname}}|
|Score/Severity|Static: 2|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0006, _mitreAttackTechnique:T1003, _mitreAttackTechnique:T1003.001, _mitreAttackTechnique:T1003.005|
## Vendors and Products
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|dstDevice_hostname|
|Normalized Schema|dstDevice_ip|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|srcDevice_hostname|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|user_username|


