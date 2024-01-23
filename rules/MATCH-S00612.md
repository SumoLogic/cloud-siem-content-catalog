# [Rules](README.md): GCP Audit Secrets Manager Activity

## Description
Administrative changes to the GCP Secrets Manager aren't overtly hostile, but are generally low volume and can be considered sensitive. These signals highlight when these actions occur and can be used in context of other suspicious activity to raise the risk of a hostile entity. Several Secrets Manager API actions are included and assessed as sensitive.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Collection|
|Apply Risk to Entities|user_username, srcDevice_ip|
|Signal Name|GCP Audit Secrets Manager Activity|
|Summary Expression|User: {{user_username}} performed action: {{action}}|
|Score/Severity|Static: 2|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0006, _mitreAttackTechnique:T1552, _mitreAttackTechnique:T1552.004, _mitreAttackTechnique:T1552.005|
## Vendors and Products
- [Google - Google Cloud Platform](../products/dcc85cfc-a698-4d09-87de-f2c723f3ad07.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|action|
|Normalized Schema|description|
|Normalized Schema|listMatches|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|user_username|


