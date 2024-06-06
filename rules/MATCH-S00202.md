# [Rules](README.md): Windows - Incoming LSASS Network Connection - Zerologon Behavior(CVE-2020-1472)

## Description
CVE-2020-1472 can be exploited by attackers to hijack enterprise servers due to Netlogon cryptographic weaknesses. The vulnerability allows an attacker to set a password for the computer account of an Active Directory Domain Controller, which can then be abused to pull credentials from the Domain Controller. This rule detects an incoming network connection made from the attacking machine to the victim Domain Controller to the LSASS process.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Execution|
|Apply Risk to Entities|device_hostname, device_ip, srcDevice_hostname, srcDevice_ip, dstDevice_ip, user_username|
|Signal Name|Incoming LSASS Network Connection - Zerologon Behavior(CVE-2020-1472)|
|Summary Expression|Zerologon activity detected on host: {{device_hostname}}|
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
|Normalized Schema|device_ip|
|Normalized Schema|dstDevice_ip|
|Direct from Record|fields['EventData.Initiated']|
|Direct from Record|fields['insertionstrings_f08']|
|Normalized Schema|file_path|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|srcDevice_hostname|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|user_username|


