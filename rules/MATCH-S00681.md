# [Rules](README.md): Mimecast Message Held

## Description
You may have a DLP policy in place to hold a message due to some security risk. It depends on the policy and this rule can be tuned to include or exclude certain policies.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Collection|
|Apply Risk to Entities|targetUser_username|
|Signal Name|Mimecast Message Held to {{targetUser_username}}|
|Summary Expression|Mimecast held an email message to {{targetUser_username}}  due to a policy.|
|Score/Severity|Static: 1|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0009, _mitreAttackTactic:TA0010, _mitreAttackTechnique:T1020, _mitreAttackTechnique:T1020.001, _mitreAttackTechnique:T1114, _mitreAttackTechnique:T1114.001, _mitreAttackTechnique:T1114.002, _mitreAttackTechnique:T1114.003|
## Vendors and Products


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|targetUser_username|


