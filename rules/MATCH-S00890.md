# [Rules](README.md): Owner Added to Azure Service Principal

## Description
An owner was added to an Azure service principal - threat actors may add owners to Azure service principals for privilege escalation or persistence avenues. Ensure this action is expected and approved.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Persistence|
|Apply Risk to Entities|user_username|
|Signal Name|Owner Added to Azure Service Principal by {{user_username}}|
|Summary Expression|Owner Added to Azure Service Principal {{application}} by {{user_username}}|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0003, _mitreAttackTechnique:T1098.001|
## Vendors and Products
- [Microsoft - Azure](../products/a1225af5-e778-4068-a9a2-47da93d1ff24.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|changeType|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|user_username|


