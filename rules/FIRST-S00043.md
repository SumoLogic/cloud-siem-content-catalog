# [Rules](README.md): First Seen pbpaste Usage from User

## Description
A user has executed a pbpaste command not seen since the baseline period. The pbpaste binary can be used to read the contents of a clipboard. This rule utilizes data from the "LOOBins" project: https://github.com/infosecB/LOOBins. more information regarding this specific binary can be found via:  https://www.loobins.io/binaries/pbpaste/

## Additional Details
|Detail|Value|
|----|----|
|Type|First Seen|
|Category|Collection|
|Apply Risk to Entities|user_username|
|Signal Name|First Seen pbpaste Usage from User|
|Summary Expression|{{user_username}} has executed a pbpaste command from {{device_hostname}}|
|Retention Window|7776000000|
|Baseline Window|1209600000|
|Baseline Type|PER_ENTITY|
|Score/Severity|Static: 2|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTechnique:T1115, _mitreAttackTactic:TA0009|
## Vendors and Products
- [CrowdStrike - FDR](../products/569a3a44-c29f-492e-bcf4-5dc04e2ab0f3.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|baseImage|
|Normalized Schema|user_username|


