# [Rules](README.md): Windows - Local System executing whoami.exe

## Description
Local system account - Suspicious System Owner/User Discovery Activity - T1033 - requires commandline auditing 4688

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Discovery|
|Apply Risk to Entities|device_hostname, device_ip, user_username|
|Signal Name|Local system execution of whoami.exe from {{device_hostname}}|
|Summary Expression|Whoami exected on host: {{device_hostname}} with command: {{commandLine}}|
|Score/Severity|Static: 2|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0007, _mitreAttackTechnique:T1033|
## Vendors and Products
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|baseImage|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|listMatches|
|Normalized Schema|parentBaseImage|
|Normalized Schema|user_username|


