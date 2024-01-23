# [Rules](README.md): Alibaba ActionTrail Secrets Manager Activity

## Description
Administrative changes to the Alibaba Secrets Manager aren't overtly hostile, but are generally low volume and can be considered sensitive.  These signals highlight when these actions occur and can be used in context of other suspicious activity to raise the risk of a hostile entity.  Several Secrets Manager API actions are included and assessed as sensitive.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Unknown/Other|
|Apply Risk to Entities|user_username, srcDevice_ip|
|Signal Name|Alibaba ActionTrail Secrets Manager Activity|
|Summary Expression|User: {{user_username}} from source IP: {{srcDevice_ip}} performed a {{action}} action|
|Score/Severity|Static: 1|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0006, _mitreAttackTechnique:T1552, _mitreAttackTechnique:T1552.004, _mitreAttackTechnique:T1552.005|
## Vendors and Products
- [Alibaba - ActionTrail](../products/79055042-52c8-4998-b201-bd2cd2dbca1f.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|action|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|user_username|


