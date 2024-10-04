# [Rules](README.md): First Seen Model ID in AWS Bedrock Put Entitlement by User

## Description
A first seen model id was observed in AWS Bedrock. The PutFoundationModelEntitlement API call grants permission to put entitlement to access a foundational model. Ensure this model is authorized to be utilized in the environment and that the user requesting access to the model is authorized to perform these actions.

## Additional Details
|Detail|Value|
|----|----|
|Type|First Seen|
|Category|Persistence|
|Apply Risk to Entities|user_username|
|Signal Name|First Seen Model ID in AWS Bedrock Put Entitlement by {{user_username}}|
|Summary Expression|First Seen Model ID in AWS Bedrock Put Entitlement from {{user_username}}|
|Retention Window|7776000000|
|Baseline Window|2592000000|
|Baseline Type|PER_ENTITY|
|Score/Severity|Static: 1|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTechnique:T1583, _mitreAttackTactic:TA0040|
## Vendors and Products
- [Amazon AWS - CloudTrail](../products/033624b0-218e-4dcb-b93f-0f1fb1806c56.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|action|
|Normalized Schema|application|
|Direct from Record|fields["responseElements.status"]|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|user_username|


