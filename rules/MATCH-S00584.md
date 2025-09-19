# [Rules](README.md): Pwndrp Access

## Description
Observes for possible attempts to download PwnDrp red team tooling

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Unknown/Other|
|Apply Risk to Entities|device_ip, srcDevice_ip, user_username|
|Signal Name|PwnDrp Access|
|Summary Expression|Observed potential pwndrop tool access on host: {{device_hostname}} from URL: {{http_url}}|
|Score/Severity|Static: 5|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0011, _mitreAttackTactic:TA0006, _mitreAttackTechnique:T1071, _mitreAttackTechnique:T1071.001, _mitreAttackTechnique:T1003|
## Vendors and Products
- [Symantec - Proxy Secure Gateway](../products/991a55cf-8c5a-49ba-ae72-6f64a002bacf.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|device_ip|
|Normalized Schema|http_url|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|user_username|


