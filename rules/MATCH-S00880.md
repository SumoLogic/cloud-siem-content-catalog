# [Rules](README.md): macOS - Entitlement Enumeration via Xattr

## Description
Threat actors may list attributes for certain files on a macOS host in order to potentially remove user prompts and execute untrusted code. This alert looks for a entitlement enumeration via the xattr binary.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Defense Evasion|
|Apply Risk to Entities|user_username|
|Signal Name|macOS - Entitlement Enumeration via Xattr|
|Summary Expression|macOS - Entitlement Enumeration via Xattr on {{device_hostname}} by {{user_username}}|
|Score/Severity|Static: 2|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0005, _mitreAttackTechnique:T1553.001|
## Vendors and Products
- [CrowdStrike - FDR](../products/569a3a44-c29f-492e-bcf4-5dc04e2ab0f3.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|baseImage|
|Normalized Schema|user_username|


