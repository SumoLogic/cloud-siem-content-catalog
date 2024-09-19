# [Rules](README.md): First Seen Kubectl Command From User

## Description
Kubectl can be used to administer Kubernetes clusters, this alert looks for a first seen Kubectl command line from a user since the baseline period.

## Additional Details
|Detail|Value|
|----|----|
|Type|First Seen|
|Category|Execution|
|Apply Risk to Entities|user_username|
|Signal Name|First Seen Kubectl Command From {{user_username}}|
|Summary Expression|{{user_username}} has issued a Kubectl command which was first seen since the baseline period on {{device_hostname}}|
|Retention Window|7776000000|
|Baseline Window|1814400000|
|Baseline Type|PER_ENTITY|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0002, _mitreAttackTechnique:T1609|
## Vendors and Products
- [CrowdStrike - FDR](../products/569a3a44-c29f-492e-bcf4-5dc04e2ab0f3.md)
- [Microsoft - Azure](../products/a1225af5-e778-4068-a9a2-47da93d1ff24.md)
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|isBlank|
|Normalized Schema|objectType|
|Normalized Schema|user_username|


