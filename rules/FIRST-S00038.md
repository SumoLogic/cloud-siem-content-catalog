# [Rules](README.md): First Seen Wget Usage from User

## Description
First Seen execution of Wget by a user from a device. The Wget tool is designed to retrieve files using various internet protocols in a programmatic manner, it is often abused by threat actors to download various files as part of broader executions. If this usage of Wget comes from an unexpected user, it is recommended that the command line value be reviewed and the URL which was used as part of Wget command be investigated.

## Additional Details
|Detail|Value|
|----|----|
|Type|First Seen|
|Category|Exfiltration|
|Apply Risk to Entities|user_username, device_hostname|
|Signal Name|First Seen Wget Usage from User|
|Summary Expression|{{user_username}} has executed a Wget command from {{device_hostname}}|
|Retention Window|7776000000|
|Baseline Window|1209600000|
|Baseline Type|PER_ENTITY|
|Score/Severity|Static: 2|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTechnique:T1048, _mitreAttackTactic:TA0010|
## Vendors and Products
- [CrowdStrike - FDR](../products/569a3a44-c29f-492e-bcf4-5dc04e2ab0f3.md)
- [Microsoft - Azure](../products/a1225af5-e778-4068-a9a2-47da93d1ff24.md)
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|baseImage|
|Normalized Schema|device_hostname|
|Normalized Schema|objectType|
|Normalized Schema|user_username|


