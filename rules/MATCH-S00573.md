# [Rules](README.md): MS Office Memory Corruption Vulnerability Exploit

## Description
Observes for exploitation of Microsoft Office Memory Corruption Vulnerability (CVE-2015-1641)

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Unknown/Other|
|Apply Risk to Entities|device_hostname, user_username|
|Signal Name|MS Office Memory Corruption Vulnerability Exploit|
|Summary Expression|CVE-2015-1641 exploit detected on {{device_hostname}}|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0005, _mitreAttackTechnique:T1036, _mitreAttackTechnique:T1036.005|
## Vendors and Products
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|baseImage|
|Normalized Schema|device_hostname|
|Normalized Schema|parentBaseImage|
|Normalized Schema|user_username|


