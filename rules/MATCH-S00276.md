# [Rules](README.md): Windows - Possible Squiblydoo Technique Observed

## Description
The Squiblydoo technique is a way for unapproved scripts to run on a machine that is setup to allow only approved scripts to run. Squiblydoo utilizes regsvr32.exe to download an XML file that contains scriptlets for executing code on the victim machine.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Defense Evasion|
|Apply Risk to Entities|device_hostname, device_ip, user_username|
|Signal Name|Windows - Possible Squiblydoo Technique Observed|
|Summary Expression|Detected possible Squiblydoo activity on host: {{device_hostname}} using command: {{commandLine}}|
|Score/Severity|Static: 2|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0005, _mitreAttackTechnique:T1218, _mitreAttackTechnique:T1218.010|
## Vendors and Products
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)
- [Tanium - Tanium Core](../products/5b49e894-92e8-45ad-8575-fe78b4f2e31b.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|baseImage|
|Normalized Schema|commandLine|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|user_username|


