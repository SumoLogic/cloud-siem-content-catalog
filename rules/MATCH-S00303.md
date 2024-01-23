# [Rules](README.md): Azure - Unauthorized OAuth Application

## Description
Alert when a non-approved OAuth Application has been identified on Azure. This rule is disabled by default as a list of approved OAuth applications is required to be enabled. The approved applications should be added to the rule logic under the 'application not in' condition.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Execution|
|Apply Risk to Entities|device_ip, user_username, srcDevice_ip|
|Signal Name|Azure - Unauthorized OAuth Application - "{{application}}"|
|Summary Expression|{{application}} is not an authorized OAuth application.|
|Score/Severity|Static: 4|
|Enabled by Default|False|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0002, _mitreAttackTactic:TA0005, _mitreAttackTactic:TA0008, _mitreAttackTechnique:T1550, _mitreAttackTechnique:T1550.001|
## Vendors and Products
- [Microsoft - Azure](../products/a1225af5-e778-4068-a9a2-47da93d1ff24.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|action|
|Normalized Schema|application|
|Normalized Schema|device_ip|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|user_username|


