# [Rules](README.md): G Suite - Access - Access Transparency

## Description
Google Access Transparency Activity Events

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Impact|
|Apply Risk to Entities|user_username|
|Signal Name|G Suite - Access - Access Transparency - "{{resource}}"|
|Summary Expression|User: {{user_username}} performed action: {{action}} on resource: {{resource}}|
|Score/Severity|Static: 2|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0009, _mitreAttackTechnique:T1530|
## Vendors and Products
- [Google - G Suite](../products/e73cd65a-7a4b-4ce9-9d73-e5d9c824c214.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|resource|
|Normalized Schema|user_username|


