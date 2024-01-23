# [Rules](README.md): First Seen AWS API Call from User

## Description
Observes for a user performing a specific API call for the first time. This may be suspicious if a user begins interacting with systems they do not typically.

## Additional Details
|Detail|Value|
|----|----|
|Type|First Seen|
|Category|Execution|
|Apply Risk to Entities|user_username|
|Signal Name|First Seen AWS API Call: {{action}} from User|
|Summary Expression|User: {{user_username}} observed executing API Call: {{action}} for service: {{application}}|
|Retention Window|7776000000|
|Baseline Window|2592000000|
|Baseline Type|PER_ENTITY|
|Score/Severity|Static: 2|
|Enabled by Default|False|
|Prototype|True|
|Tags|_mitreAttackTactic:TA0002|
## Vendors and Products
- [Amazon AWS - CloudTrail](../products/033624b0-218e-4dcb-b93f-0f1fb1806c56.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|action|
|Direct from Record|fields["userIdentity.type"]|
|Normalized Schema|isEmpty|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|user_username|
|Normalized Schema|user_username_role|


