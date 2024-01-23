# [Rules](README.md): G Suite - Drive - Drive Open To Public

## Description
Google Drive resource shared publicly

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Exfiltration|
|Apply Risk to Entities|user_username|
|Signal Name|G Suite - Drive Open To Public|
|Summary Expression|User: {{user_username}} performed action: {{action}} on resource: {{resource}}|
|Score/Severity|Static: 4|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0009, _mitreAttackTechnique:T1530|
## Vendors and Products
- [Google - G Suite](../products/e73cd65a-7a4b-4ce9-9d73-e5d9c824c214.md)


## Fields Used

|Origin|Field|
|----|----|
|Direct from Record|fields['event.parameters.visibility']|
|Direct from Record|fields['events.parameters.visibility']|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|user_username|


