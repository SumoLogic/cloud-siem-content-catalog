# [Rules](README.md): Azure Conditional Access Policy Disabled

## Description
Azure Conditional Access policies control various aspects of access to Azure resources, including the requirement for multi or strong authentication, disabling of conditional policies outside of expected administrative activity should be investigated for legitimacy.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Privilege Escalation|
|Apply Risk to Entities|user_username|
|Signal Name|Azure Conditional Access Policy Disabled|
|Summary Expression|{{user_username}} has disabled an Azure Conditional Access Policy named {{application}}|
|Score/Severity|Static: 5|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0004, _mitreAttackTactic:TA0005, _mitreAttackTechnique:T1078.004, _mitreAttackTechnique:T1078|
## Vendors and Products
- [Microsoft - Azure](../products/a1225af5-e778-4068-a9a2-47da93d1ff24.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|action|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_product|
|Normalized Schema|user_username|


