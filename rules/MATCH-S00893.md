# [Rules](README.md): Secret Added to Azure Service Principal

## Description
Secrets can be added to Azure Service Principals as a persistence mechanism. The properties.targetResources.1.modifiedProperties.1.newValue field will have details regarding the secret or certificate added.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Persistence|
|Apply Risk to Entities|user_username|
|Signal Name|Certificate or Secret Added to Azure Service Principal {{targetUser_username_raw}}|
|Summary Expression|A new secret has been added to an Azure Service Principal|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|True|
|Tags|_mitreAttackTactic:TA0003, _mitreAttackTechnique:T1098.001|
## Vendors and Products
- [Microsoft - Azure](../products/a1225af5-e778-4068-a9a2-47da93d1ff24.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|changeType|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|targetUser_username_raw|
|Normalized Schema|user_username|


