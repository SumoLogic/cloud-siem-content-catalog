# [Rules](README.md): NinjaCopy Usage Detected

## Description
NinjaCopy is a legacy PowerShell tool that can copy files from an NTFS volume in a manner that bypasses SACL auditing as well as DACL controls such as only allowing SYSTEM to open a file. This tool is often used to exfiltrate the Active Directory database (NTDS.dit) file from domain controllers in order to extract credential material. Usage of this tool in an environment should be considered highly suspciious.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Defense Evasion|
|Apply Risk to Entities|device_hostname|
|Signal Name|NinjaCopy Usage Detected on {{device_hostname}}|
|Summary Expression|NinjaCopy Usage Detected on {{device_hostname}} from the {{baseImage}} process|
|Score/Severity|Static: 4|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0005, _mitreAttackTechnique:T1006|
## Vendors and Products


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|device_hostname|


