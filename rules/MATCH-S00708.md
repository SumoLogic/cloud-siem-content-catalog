# [Rules](README.md): AzureDevOps - Project Visibility Changed to Public

## Description
This rule generates a signal when an Azure DevOps project has its visibility changed to a public project.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Collection|
|Apply Risk to Entities|srcDevice_ip, user_username|
|Signal Name|AzureDevOps - Project Visibility Changed to Public|
|Summary Expression|AzureDevOps - Project Visibility Changed to Public from IP: {{srcDevice_ip}} by User: {{user_username}}|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0009, _mitreAttackTechnique:T1213, _mitreAttackTechnique:T1213.003|
## Vendors and Products
- [Microsoft - Azure](../products/a1225af5-e778-4068-a9a2-47da93d1ff24.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|action|
|Normalized Schema|description|
|Direct from Record|fields['properties.Data.PreviousProjectVisibility']|
|Direct from Record|fields['properties.Data.ProjectVisibility']|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|user_username|


