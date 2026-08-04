# [Rules](README.md): Normalized Identity Detection

## Description
Passes through an identity or access anomaly detection (e.g. Azure risky user, Google Workspace, Slack, Okta) and adjusts the severity accordingly based on the severity provided in the log.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Initial Access|
|Apply Risk to Entities|user_username, targetUser_username, user_email, srcDevice_ip, http_userAgent|
|Signal Name|{{metadata_vendor}} {{metadata_product}} - {{threat_signalName}}|
|Summary Expression|Identity risk: {{threat_signalName}} for {{user_username}}|
|Score/Severity|None|
|Enabled by Default|True|
|Prototype|False|
|Tags||
## Vendors and Products
- [Microsoft - Azure](../products/a1225af5-e778-4068-a9a2-47da93d1ff24.md)
- [Slack - Slack](../products/79da6240-7617-49c8-b130-96278579766e.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|http_userAgent|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|normalizedSeverity|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|targetUser_username|
|Normalized Schema|threat_ruleType|
|Normalized Schema|threat_signalName|
|Normalized Schema|user_email|
|Normalized Schema|user_username|


