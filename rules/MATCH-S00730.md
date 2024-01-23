# [Rules](README.md): Registry Modification - Code Signing

## Description
The Driver Signature Enforcement functionality in Windows ensures that only approved, unaltered programs are able to run on a system. Modifications to this policy can indicate an attempt to bypass these built-in protections. Tuning for this rule may be required for developer machines as code signing protections often interfere with the software development process.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Defense Evasion|
|Apply Risk to Entities|device_hostname, device_ip, user_username|
|Signal Name|Registry Modification - Code Signing|
|Summary Expression|User {{user_username}} modified registry key {{changeTarget}} on host {{device_hostname}}|
|Score/Severity|Static: 2|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0005, _mitreAttackTechnique:T1553.006|
## Vendors and Products
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|changeTarget|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|user_username|


