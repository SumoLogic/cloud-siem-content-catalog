# [Rules](README.md): HAR file creation observed on host

## Description
HAR files contain session telemetry and network traffic. These file types are typically generated using the "developer tools" options on modern browsers like Chrome, Edge or Firefox. These files may contain various sensitive data such as session keys, tokens or cookies which may be extracted by a threat actor in order to access systems  which the keys, tokens or cookies in the HAR files have access to. Ensure that this operation is expected and ensure to sanitize the HAR file of any sensitive credential material.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Collection|
|Apply Risk to Entities|device_hostname|
|Signal Name|HAR file creation observed on {{device_hostname}}|
|Summary Expression|{{user_username}} has created a HAR file on {{device_hostname}}|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0009, _mitreAttackTechnique:T1185, _mitreAttackTactic:TA0006, _mitreAttackTechnique:T1539, _mitreAttackTactic:TA0005, _mitreAttackTechnique:T1550.004|
## Vendors and Products
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|action|
|Normalized Schema|device_hostname|


