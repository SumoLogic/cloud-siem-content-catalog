# [Rules](README.md): GitHub - First Seen Activity From Country for User

## Description
Detects GitHub user activity from a new country. User account compromises can be detected through unusual geolocation in some cases. To lower possible false positives, a tuning expression for expected country names or codes can be added,. This detection was developed utilizing GitHub Enterprise Audit logging. Refer to https://help.sumologic.com/docs/integrations/app-development/github/#collecting-logs-for-github for instructions on ingesting GitHub Enterprise Audit logs.

## Additional Details
|Detail|Value|
|----|----|
|Type|First Seen|
|Category|Credential Access|
|Apply Risk to Entities|user_username|
|Signal Name|GitHub - First Seen Activity from new country {{srcDevice_ip_countryName}} by {{user_username}}|
|Summary Expression|Detected activity {{action}}  performed by user {{user_username}}  from {{srcDevice_ip}}  in {{srcDevice_ip_countryName}}|
|Retention Window|7776000000|
|Baseline Window|2592000000|
|Baseline Type|PER_ENTITY|
|Score/Severity|Static: 2|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0006, _mitreAttackTechnique:T1078|
## Vendors and Products
- [Github - GitHub Enterprise Audit](../products/e3c8bd8b-6ed8-4332-944d-d0f5dfc462df.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|metadata_product|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|srcDevice_ip_countryName|
|Normalized Schema|srcDevice_ip_isInternal|
|Normalized Schema|user_username|


