# [Rules](README.md): First Seen IP Address Associated with User for a Successful Azure AD Sign In Event

## Description
Detects when a new IP address is associated with a successful Azure sign in event for a particular username since the baseline period.

## Additional Details
|Detail|Value|
|----|----|
|Type|First Seen|
|Category|Initial Access|
|Apply Risk to Entities|user_username|
|Signal Name|First Seen IP Address: {{device_ip}} Associated with User for a Successful Azure AD Sign In Event|
|Summary Expression|{{user_username}} has successfully signed into an Azure resource with a first seen IP address of {{device_ip}} since the baseline period.|
|Retention Window|7776000000|
|Baseline Window|1814400000|
|Baseline Type|PER_ENTITY|
|Score/Severity|Static: 1|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0001, _mitreAttackTechnique:T1078.004|
## Vendors and Products
- [Microsoft - Azure](../products/a1225af5-e778-4068-a9a2-47da93d1ff24.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|device_ip|
|Normalized Schema|errorCode|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_product|
|Normalized Schema|objectType|
|Normalized Schema|success|
|Normalized Schema|user_username|


