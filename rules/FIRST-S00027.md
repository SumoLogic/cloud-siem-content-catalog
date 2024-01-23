# [Rules](README.md): First Seen InstallUtil Allow List Bypass From User

## Description
This rule looks for a suspicious InstallUtil outgoing network connection from the InstallUtil process, indicating potentially malicious use of the InstallUtil binary.

## Additional Details
|Detail|Value|
|----|----|
|Type|First Seen|
|Category|Defense Evasion|
|Apply Risk to Entities|device_hostname, user_username|
|Signal Name|First Seen InstallUtil Allow List Bypass From User|
|Summary Expression|First seen InstallUtil network connection detected on host: {{device_hostname}} by user: {{user_username}}|
|Retention Window|7776000000|
|Baseline Window|1209600000|
|Baseline Type|GLOBAL|
|Score/Severity|Static: 2|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0005, _mitreAttackTechnique:T1218, _mitreAttackTechnique:T1218.004|
## Vendors and Products
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|baseImage|
|Normalized Schema|device_hostname|
|Direct from Record|fields['EventData.Initiated']|
|Normalized Schema|user_username|


