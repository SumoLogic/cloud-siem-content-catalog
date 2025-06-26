# [Rules](README.md): First Seen networksetup Usage from User

## Description
A user has executed a networksetup command not seen since the baseline period. The networksetup binary can be used to change and discover network settings on a Unix or macOS host. This rule utilizes data from the "LOOBins" project: https://github.com/infosecB/LOOBins

## Additional Details
|Detail|Value|
|----|----|
|Type|First Seen|
|Category|Discovery|
|Apply Risk to Entities|user_username|
|Signal Name|First Seen networksetup Usage from User|
|Summary Expression|{{user_username}} has executed a networksetup command on host: {{device_hostname}}|
|Retention Window|7776000000|
|Baseline Window|1209600000|
|Baseline Type|PER_ENTITY|
|Score/Severity|Static: 2|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0007, _mitreAttackTechnique:T1082|
## Vendors and Products
- [CrowdStrike - FDR](../products/569a3a44-c29f-492e-bcf4-5dc04e2ab0f3.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|baseImage|
|Normalized Schema|user_username|


