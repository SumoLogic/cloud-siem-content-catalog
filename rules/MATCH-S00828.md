# [Rules](README.md): Office 365 Exchange Transport Rule Created

## Description
Threat actors may create, update or otherwise modify various Office 365 inbox rules to delete sensitive emails - such as those originating from security teams - or automatically forward emails to a mailbox in their control.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Collection|
|Apply Risk to Entities|user_username|
|Signal Name|Office 365 Exchange Transport Rule Created|
|Summary Expression|{{user_username}} has created an Office 365 Transport Rule|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0009, _mitreAttackTechnique:T1114.003|
## Vendors and Products
- [Microsoft - Office 365](../products/d3ed003d-5ddd-4c7a-bea5-63eae6311833.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|action|
|Normalized Schema|metadata_product|
|Normalized Schema|user_username|


