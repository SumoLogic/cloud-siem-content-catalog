# [Rules](README.md): GCP Audit IAM DeleteServiceAccount Observed

## Description
Identifies when a service account is deleted in Google Cloud Platform (GCP). A service account is a special type of account used by an application or a virtual machine (VM) instance, not a person. Applications use service accounts to make authorized API calls, authorized as either the service account itself, or as G Suite or Cloud Identity users through domain-wide delegation. An adversary may delete a service account in order to disrupt their target's business operations.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Impact|
|Apply Risk to Entities|user_username, srcDevice_ip|
|Signal Name|GCP Audit IAM DeleteServiceAccount Observed|
|Summary Expression|User: {{user_username}} performed action: {{action}}|
|Score/Severity|Static: 1|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTechnique:T1531, _mitreAttackTactic:TA0040|
## Vendors and Products
- [Google - Google Cloud Platform](../products/dcc85cfc-a698-4d09-87de-f2c723f3ad07.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|action|
|Normalized Schema|listMatches|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|user_username|


