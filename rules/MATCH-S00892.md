# [Rules](README.md): Value Added to Azure NSG Group

## Description
This alert looks for a value being added to an Azure Network Security Group (NSG) successfully. Depending on the environment, other Azure services such as Azure FIrewall may provide egress and ingress controls. Ensure this activity is authorized and expected. The raw data for the event contains the exact values being modified.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Defense Evasion|
|Apply Risk to Entities|user_username|
|Signal Name|Value Added to Azure NSG Group|
|Summary Expression|An Azure Network Security Group (NSG) has been modified with a value being added|
|Score/Severity|Static: 2|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0005, _mitreAttackTechnique:T1562.007|
## Vendors and Products
- [Microsoft - Azure](../products/a1225af5-e778-4068-a9a2-47da93d1ff24.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|action|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_product|
|Normalized Schema|success|
|Normalized Schema|user_username|


