# [Rules](README.md): First Seen AppID Generating MailItemsAccessed Event from User

## Description
This alert looks at a first seen application ID accessing an Office 365/Exchange mail box item The MailItemsAccessed may not always be enabled within an Entra/Azure/Office 365 tenant and is dependent on Microsoft licensing requirements. See the following guide from CISA for additional information on this event type and investigation steps: https://www.cisa.gov/news-events/cybersecurity-advisories/aa23-193a

## Additional Details
|Detail|Value|
|----|----|
|Type|First Seen|
|Category|Collection|
|Apply Risk to Entities|user_username|
|Signal Name|First Seen AppId Generating MailItemsAccessed Event from {{user_username}}|
|Summary Expression|A First Seen AppId was observed as accessing an Office 365 mail item since the baseline period.|
|Retention Window|7776000000|
|Baseline Window|1209600000|
|Baseline Type|PER_ENTITY|
|Score/Severity|Static: 1|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0009, _mitreAttackTechnique:T1114|
## Vendors and Products
- [Microsoft - Office 365](../products/d3ed003d-5ddd-4c7a-bea5-63eae6311833.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|action|
|Normalized Schema|metadata_product|
|Normalized Schema|user_username|


