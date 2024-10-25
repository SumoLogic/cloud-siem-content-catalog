# [Rules](README.md): Windows Credential Editor (WCE) in use

## Description
Looks for the possible use of Windows Credential Editor, a common open-source tool used for pass-the-hash amongst other attacks.  This detection examins the import hash (aka imphash) as well as process start identifiers associated with the tool.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Privilege Escalation|
|Apply Risk to Entities|device_hostname, device_ip, user_username|
|Signal Name|Windows Credential Editor (WCE) in use|
|Summary Expression|Pass the hash activity observed on host: {{device_hostname}}|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0004, _mitreAttackTactic:TA0006, _mitreAttackTechnique:T1003|
## Vendors and Products
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|commandLine|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|file_hash_imphash|
|Normalized Schema|parentBaseImage|
|Normalized Schema|user_username|


