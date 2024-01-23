# [Rules](README.md): Potential Reconnaissance Obfuscation

## Description
From Solorigate TTPs: Firewall rules were added via command line to reduce noise from subsequent reconnaissance using NSLOOKUP and ADFIND.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Defense Evasion|
|Apply Risk to Entities|device_hostname, user_username|
|Signal Name|Potential Reconnaissance Obfuscation|
|Summary Expression|Potential reconnaissance obfuscation activity on host: {{device_hostname}}|
|Score/Severity|Static: 5|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0005, _mitreAttackTechnique:T1562.001, _mitreAttackTechnique:T1562.002, _mitreAttackTechnique:T1562.004, _mitreAttackTechnique:T1562.006|
## Vendors and Products
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|commandLine|
|Normalized Schema|device_hostname|
|Normalized Schema|user_username|


