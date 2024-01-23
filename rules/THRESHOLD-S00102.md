# [Rules](README.md): Domain Password Attack

## Description
Detects multiple failed login attempts from a single source with unique usernames over a 1 hour timeframe. This is designed to catch attacks leveraging domain resources to attempt credential validation. The threshold and time frame can be adjusted based on the customer's environment.

## Additional Details
|Detail|Value|
|----|----|
|Type|Threshold|
|Category|Initial Access|
|Apply Risk to Entities|srcDevice_hostname, srcDevice_ip|
|Signal Name|Domain Password Attack|
|Summary Expression|Password attack from IP: {{srcDevice_ip}} host: {{srcDevice_hostname}}|
|Threshold Count|50|
|Threshold Window|60m|
|Score/Severity|Static: 2|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0001, _mitreAttackTactic:TA0006, _mitreAttackTechnique:T1110, _mitreAttackTechnique:T1078, _mitreAttackTechnique:T1078.001, _mitreAttackTechnique:T1078.002, _mitreAttackTechnique:T1078.003, _mitreAttackTechnique:T1078.004, _mitreAttackTechnique:T1586, _mitreAttackTechnique:T1586.001, _mitreAttackTechnique:T1586.002, _mitreAttackTactic:TA0008, _mitreAttackTechnique:T1110.003, _mitreAttackTechnique:T1110.002, _mitreAttackTechnique:T1110.001|
## Vendors and Products
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|device_hostname|
|Normalized Schema|listMatches|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|normalizedAction|
|Normalized Schema|objectType|
|Normalized Schema|srcDevice_hostname|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|success|
|Normalized Schema|user_username|


