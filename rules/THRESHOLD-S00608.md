# [Rules](README.md): Alibaba ActionTrail Unauthorized API Calls

## Description
An IAM account sent multiple requests to perform a wide distinct number of Alibaba Cloud actions in a short time frame while receiving error codes. This could indicate an account attempting to enumerate their access across the Alibaba account.

## Additional Details
|Detail|Value|
|----|----|
|Type|Threshold|
|Category|Initial Access|
|Apply Risk to Entities|user_username, srcDevice_ip|
|Signal Name|Alibaba ActionTrail Unauthorized API Calls|
|Summary Expression|User: {{user_username}} from source IP: {{srcDevice_ip}} attempted multiple actions resulting in error codes|
|Threshold Count|2|
|Threshold Window|60m|
|Score/Severity|Static: 6|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0006, _mitreAttackTechnique:T1552, _mitreAttackTechnique:T1552.005|
## Vendors and Products
- [Alibaba - ActionTrail](../products/79055042-52c8-4998-b201-bd2cd2dbca1f.md)


## Fields Used

|Origin|Field|
|----|----|
|Direct from Record|fields['errorCode']|
|Direct from Record|fields['eventType']|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|user_username|


