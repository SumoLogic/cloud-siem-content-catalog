# [Rules](README.md): GCP Audit Unauthorized API Calls

## Description
An IAM account sent multiple requests to perform a wide distinct number of GCP Cloud actions in a short time frame while receiving the error codes. This could indicate an account attempting to enumerate their access across the GCP account.

## Additional Details
|Detail|Value|
|----|----|
|Type|Threshold|
|Category|Initial Access|
|Apply Risk to Entities|user_username, srcDevice_ip|
|Signal Name|GCP Audit Unauthorized API Calls|
|Summary Expression|User: {{user_username}} attempted to perform multiple distinct actions with failure|
|Threshold Count|2|
|Threshold Window|60m|
|Score/Severity|Static: 6|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0006, _mitreAttackTechnique:T1552, _mitreAttackTechnique:T1552.005|
## Vendors and Products
- [Google - Google Cloud Platform](../products/dcc85cfc-a698-4d09-87de-f2c723f3ad07.md)


## Fields Used

|Origin|Field|
|----|----|
|Direct from Record|fields['message.data.protoPayload.response.error.code']|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|user_username|


