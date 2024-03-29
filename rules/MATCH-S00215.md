# [Rules](README.md): Auth0 - High Risk Event

## Description
Passthrough rule for high risk events generated by Auth0

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Initial Access|
|Apply Risk to Entities|device_ip, user_username|
|Signal Name|Auth0 - High Risk Event|
|Summary Expression|{{description}}|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0001, _mitreAttackTechnique:T1078, _mitreAttackTechnique:T1078.004|
## Vendors and Products


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|device_ip|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_product|
|Normalized Schema|user_username|


