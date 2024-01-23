# [Rules](README.md): Unauthorized Access Attempt Detected

## Description
Most login failures are due to failed passwords. Login failure to sensitive systems where the users simply aren't authorized, though, can indicate malicious intent.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Credential Access|
|Apply Risk to Entities|device_hostname, device_ip, user_username|
|Signal Name|Unauthorized Access Attempt Detected|
|Summary Expression|Unauthorized access attempts from user: {{user_username}} on host: {{device_hostname}}|
|Score/Severity|Static: 2|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0006, _mitreAttackTechnique:T1110, _mitreAttackTechnique:T1110.001, _mitreAttackTechnique:T1110.002, _mitreAttackTechnique:T1110.003, _mitreAttackTechnique:T1110.004|
## Vendors and Products
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|errorCode|
|Direct from Record|fields['insertionstrings_f10']|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|user_username|


