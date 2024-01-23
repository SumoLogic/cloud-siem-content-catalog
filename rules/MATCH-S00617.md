# [Rules](README.md): GCP GCPloit Exploitation Framework Used

## Description
Generates a signal when the GCPloit exploitation framework is detected. This framework can be used to escalate privileges and move laterally from compromised high privilege accounts.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Initial Access|
|Apply Risk to Entities|user_username, srcDevice_ip|
|Signal Name|GCP GCPloit Exploitation Framework Used|
|Summary Expression|GCPloit exploitation detected from IP {{srcDevice_ip}}|
|Score/Severity|Static: 6|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTechnique:T1190, _mitreAttackTactic:TA0001, _mitreAttackTactic:TA0008, _mitreAttackTactic:TA0004, _mitreAttackTechnique:T1068|
## Vendors and Products
- [Google - Google Cloud Platform](../products/dcc85cfc-a698-4d09-87de-f2c723f3ad07.md)


## Fields Used

|Origin|Field|
|----|----|
|Direct from Record|fields['message.data.protoPayload.request.function.timeout']|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|user_username|


