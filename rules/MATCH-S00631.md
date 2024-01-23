# [Rules](README.md): GCP Audit IAM Custom Role Deletion

## Description
Identifies an Identity and Access Management (IAM) role deletion in Google Cloud Platform (GCP). A role contains a set of permissions that allows you to perform specific actions on Google Cloud resources. An adversary may delete an IAM role to inhibit access to accounts utilized by legitimate users.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Impact|
|Apply Risk to Entities|user_username, srcDevice_ip|
|Signal Name|GCP Audit IAM Custom Role Deletion|
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


