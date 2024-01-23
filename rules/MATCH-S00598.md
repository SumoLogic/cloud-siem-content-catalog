# [Rules](README.md): Alibaba ActionTrail Logging Configuration Change Observed

## Description
Changing the configuration of logging to any mission-critical service or platform should be closely monitored.  This signal identifies when Alibaba logging configurations have been changed.  The severity of signals increases depending on the type of action observed.  For instance disabling/deleting logs is a higher severity than enabling logs.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Unknown/Other|
|Apply Risk to Entities|srcDevice_ip, user_username|
|Signal Name|Alibaba ActionTrail Logging Configuration Change Observed|
|Summary Expression|User: {{user_username}} from source IP: {{srcDevice_ip}} performed a {{action}} action|
|Score/Severity|Dynamic: 1 or 2 or 4|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0002, _mitreAttackTactic:TA0005, _mitreAttackTechnique:T1489, _mitreAttackTechnique:T1578, _mitreAttackTechnique:T1562, _mitreAttackTechnique:T1578.004, _mitreAttackTechnique:T1562.008|
## Vendors and Products
- [Alibaba - ActionTrail](../products/79055042-52c8-4998-b201-bd2cd2dbca1f.md)


## Dynamic Signal Score/Severity Translation

The default score of `1` is used as a catch all if none of the translations are met.

|Schema Field|Field Value|Score/Severity|
|------------|-----------|--------------|
|action|CreateTrail|1|
|action|UpdateTrail|2|
|action|DeleteTrail|4|
|action|StartLogging|1|
|action|StopLogging|4|
## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|action|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|user_username|


