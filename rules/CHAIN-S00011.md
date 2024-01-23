# [Rules](README.md): Potential InstallUtil Allow List Bypass

## Description
This rule looks for a suspicious InstallUtil command line followed by an observed outgoing network connection from the InstallUtil process, indicating potentially malicious use of the InstallUtil binary.

## Additional Details
|Detail|Value|
|----|----|
|Type|Chain|
|Category|Defense Evasion|
|Apply Risk to Entities|device_hostname, user_username|
|Signal Name|Potential InstallUtil Allow List Bypass|
|Summary Expression|Potential InstallUtil Allow List Bypass followed by an InstallUtil network connection detected on host: {{device_hostname}} by user: {{user_username}}|
|Score/Severity|Static: 4|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0005, _mitreAttackTechnique:T1218, _mitreAttackTechnique:T1218.004|
## Vendors and Products


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|baseImage|
|Normalized Schema|device_hostname|
|Direct from Record|fields["EventData.Initiated"]|
|Normalized Schema|user_username|


