# [Rules](README.md): macOS - csrutil status Usage Detected

## Description
The csrutil binary should be rarely used by regular end-users and is designed to return the status of System Integrity Protection (SIP) - ensure this execution is expected or performed by an administrator or adminstrative function/automation.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Discovery|
|Apply Risk to Entities|user_username, device_hostname|
|Signal Name|macOS - csrutil Usage Detected|
|Summary Expression|macOS - csrutil Usage Detected on {{device_hostname}} executed by {{user_username}}|
|Score/Severity|Static: 0|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTechnique:T1082, _mitreAttackTactic:TA0007|
## Vendors and Products
- [CrowdStrike - FDR](../products/569a3a44-c29f-492e-bcf4-5dc04e2ab0f3.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|baseImage|
|Normalized Schema|device_hostname|
|Normalized Schema|matches|
|Normalized Schema|parentBaseImage|
|Normalized Schema|user_username|


