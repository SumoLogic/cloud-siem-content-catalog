# [Rules](README.md): Suspicious chmod Execution

## Description
This alert looks for a "chmod" execution on a file that is found on the /tmp directory of a Linux or macOS host. Threat actors may download and copy files to this directory and add execution bits or change permissions on these files.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Defense Evasion|
|Apply Risk to Entities|user_username, device_hostname|
|Signal Name|Suspicious chmod Execution|
|Summary Expression|Suspicious chmod Execution on {{device_hostname}} by {{user_username}}|
|Score/Severity|Static: 2|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0005, _mitreAttackTechnique:T1222.002|
## Vendors and Products
- [CrowdStrike - FDR](../products/569a3a44-c29f-492e-bcf4-5dc04e2ab0f3.md)
- [Linux - Sysmon for Linux](../products/b238758d-ade8-41d2-b32d-c99159e9fd74.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|baseImage|
|Normalized Schema|commandLine|
|Normalized Schema|device_hostname|
|Direct from Record|fields["exec_env.env.PWD"]|
|Normalized Schema|user_username|


