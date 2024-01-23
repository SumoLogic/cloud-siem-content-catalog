# [Rules](README.md): GCP Bucket Open

## Description
A GCP request occurred to either create a new public or open bucket. While there are some use cases for GCP S3 public buckets, most are generally private. The security operations center should have a strong understanding of which buckets are allowed to be public.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Defense Evasion|
|Apply Risk to Entities|user_username, srcDevice_ip|
|Signal Name|GCP Bucket Open|
|Summary Expression|User: {{user_username}} made storage bucket public|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0009, _mitreAttackTechnique:T1530|
## Vendors and Products
- [Google - Google Cloud Platform](../products/dcc85cfc-a698-4d09-87de-f2c723f3ad07.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|action|
|Direct from Record|fields['message.data.protoPayload.serviceData.policyDelta.bindingDeltas.1.action']|
|Direct from Record|fields['message.data.protoPayload.serviceData.policyDelta.bindingDeltas.1.member']|
|Direct from Record|fields['message.data.resource.type']|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|user_username|


