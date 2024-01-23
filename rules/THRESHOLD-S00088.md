# [Rules](README.md): GCP Audit Reconnaissance Activity

## Description
This signal identifies GCP API GET and LIST actions that when observed in combination could indicate an actors intent to enumerate the environment. These events are generally benign, and occur during normal operations. Use this signal as context around an unfolding security story.

## Additional Details
|Detail|Value|
|----|----|
|Type|Threshold|
|Category|Unknown/Other|
|Apply Risk to Entities|user_username, srcDevice_ip|
|Signal Name|GCP Audit Reconnaissance Activity|
|Summary Expression|User: {{user_username}} performed GCP recon related actions|
|Threshold Count|5|
|Threshold Window|60m|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0007, _mitreAttackTechnique:T1069, _mitreAttackTechnique:T1087, _mitreAttackTechnique:T1526, _mitreAttackTechnique:T1087.004, _mitreAttackTechnique:T1069.003|
## Vendors and Products
- [Google - Google Cloud Platform](../products/dcc85cfc-a698-4d09-87de-f2c723f3ad07.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|action|
|Normalized Schema|description|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|user_username|


