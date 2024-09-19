# [Rules](README.md): Windows Credential Editor (WCE) Tool Use Detected

## Description
This signal inciates that an indicator in the windows registry was found that indicates the Windows Credential Editor (WCE) tool may be in use.  This tool use is highly suspicious and can indicate lateral movement attempts (pass-the-hash etc.)  REF: https://www.ampliasecurity.com/research/windows-credentials-editor/

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Privilege Escalation|
|Apply Risk to Entities|device_hostname, device_ip, user_username|
|Signal Name|Windows Credential Editor (WCE) Tool Use Detected|
|Summary Expression|Pass the hash activity observed on host: {{device_hostname}}|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0004, _mitreAttackTactic:TA0006, _mitreAttackTactic:TA0005, _mitreAttackTactic:TA0008, _mitreAttackTechnique:T1003, _mitreAttackTechnique:T1550, _mitreAttackTechnique:T1550.002|
## Vendors and Products
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|baseImage|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|file_path|
|Normalized Schema|user_username|


