# [Rules](README.md): Alibaba ActionTrail Root Login

## Description
This signal detects when a successful root account login occurred within an Alibaba account. This privileged account should seldomly be used within an Alibaba cloud environment.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Unknown/Other|
|Apply Risk to Entities|user_username, srcDevice_ip|
|Signal Name|Alibaba ActionTrail Root Login|
|Summary Expression|User: {{user_username}} from source IP: {{srcDevice_ip}} logged in as root|
|Score/Severity|Static: 5|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0001, _mitreAttackTactic:TA0003, _mitreAttackTactic:TA0004, _mitreAttackTactic:TA0005, _mitreAttackTactic:TA0042, _mitreAttackTechnique:T1078, _mitreAttackTechnique:T1078.004, _mitreAttackTechnique:T1078.001|
## Vendors and Products
- [Alibaba - ActionTrail](../products/79055042-52c8-4998-b201-bd2cd2dbca1f.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|action|
|Direct from Record|fields['errorCode']|
|Direct from Record|fields['userIdentity.type']|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|user_username|


