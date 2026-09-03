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
- [Box - Box](../products/0472f22e-e3fa-4c9f-a529-8355f671927e.md)
- [CrowdStrike - Falcon](../products/840c72e0-4e47-41e7-9b93-31f55d12f07d.md)
- [Google - Google Workspace](../products/e73cd65a-7a4b-4ce9-9d73-e5d9c824c214.md)
- [Microsoft - Azure](../products/a1225af5-e778-4068-a9a2-47da93d1ff24.md)
- [Microsoft - Graph Identity Protection API](../products/4da7313c-5123-4eae-bb84-5d868fc55a74.md)
- [Okta - Single Sign-On](../products/51278354-d6b5-4c8e-a8fd-8197df334e67.md)
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


