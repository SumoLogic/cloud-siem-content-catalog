# [Rules](README.md): First Seen mdfind Usage from User

## Description
A user has executed a mdfind command not seen since the baseline period. The mdfind binary can be used to find passwords and other sensitive info on the host  system. This rule utilizes data from the "LOOBins" project: https://github.com/infosecB/LOOBins - more information regarding this specific binary can be found via: https://www.loobins.io/binaries/mdfind/

## Additional Details
|Detail|Value|
|----|----|
|Type|First Seen|
|Category|Discovery|
|Apply Risk to Entities|user_username|
|Signal Name|First Seen mdfind Usage from User|
|Summary Expression|{{user_username}} has executed a mdfind command from {{device_hostname}}|
|Retention Window|7776000000|
|Baseline Window|1209600000|
|Baseline Type|PER_ENTITY|
|Score/Severity|Static: 2|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0007, _mitreAttackTechnique:T1083|
## Vendors and Products
- [CrowdStrike - FDR](../products/569a3a44-c29f-492e-bcf4-5dc04e2ab0f3.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|baseImage|
|Normalized Schema|com.grammarly.ProjectLlama|
|Normalized Schema|commandLine|
|Normalized Schema|matches|
|Normalized Schema|parentBaseImage|
|Normalized Schema|user_username|


