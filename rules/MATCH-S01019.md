# [Rules](README.md): Threat Intel - Matched User Email

## Description
Detects email addresses associated with known malicious actor(s) or campaign(s) as designated by a threat intelligence provider.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Threat Intelligence|
|Apply Risk to Entities|user_username, user_email, targetUser_username, targetUser_email|
|Signal Name|Threat Intel - Matched Email|
|Summary Expression|The record contains an email address associated with a threat intelligence feed: {{user_email}}|
|Score/Severity|Static: 1|
|Enabled by Default|True|
|Prototype|False|
|Tags||
## Vendors and Products
- [Abnormal Security - Abnormal Security](../products/2b79254e-8017-4dbf-8e39-590132172a7d.md)
- [Google - BigQuery](../products/a67d97fe-6e68-4cfb-9500-cfc5492da565.md)
- [Google - Google Workspace](../products/e73cd65a-7a4b-4ce9-9d73-e5d9c824c214.md)
- [Microsoft - Azure](../products/a1225af5-e778-4068-a9a2-47da93d1ff24.md)
- [Microsoft - Defender Advanced Hunting](../products/3382523e-2072-41bd-b50b-6b148957d0b0.md)
- [Okta - Single Sign-On](../products/51278354-d6b5-4c8e-a8fd-8197df334e67.md)
- [Zoom - Zoom](../products/ad8d40a9-ee64-4615-bd92-aa964b4ae3b0.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|targetUser_email|
|Normalized Schema|targetUser_username|
|Normalized Schema|user_email|
|Normalized Schema|user_username|


