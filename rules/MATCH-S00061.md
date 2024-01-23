# [Rules](README.md): Zscaler - Allowed Elevated Risk Score Events

## Description
Observes for a high risk event that was permitted by ZScaler

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Command and Control|
|Apply Risk to Entities|device_hostname, device_ip, srcDevice_hostname, srcDevice_ip, user_username|
|Signal Name|Zscaler - Allowed Elevated Risk Score Event|
|Summary Expression|Zscaler generated a record with an elevated risk score of {{fields['riskscore']}} from the user {{user_username}} and IP address {{srcDevice_ip}}.|
|Score/Severity|Dynamic: 1 or 2 or 3|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0011, _mitreAttackTechnique:T1071, _mitreAttackTechnique:T1071.001|
## Vendors and Products
- [Zscaler - Nanolog Streaming Service](../products/6299d728-14f7-455e-85c5-ea8ec65a654a.md)


## Dynamic Signal Score/Severity Translation

The default score of `1` is used as a catch all if none of the translations are met.

|Schema Field|Field Value|Score/Severity|
|------------|-----------|--------------|
|fields['riskscore']|75|2|
|fields['riskscore']|80|2|
|fields['riskscore']|85|2|
|fields['riskscore']|90|2|
|fields['riskscore']|95|3|
|fields['riskscore']|100|3|
## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|action|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Direct from Record|fields['riskscore']|
|Normalized Schema|metadata_vendor|
|Normalized Schema|srcDevice_hostname|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|user_username|


