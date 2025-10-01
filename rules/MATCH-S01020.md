# [Rules](README.md): Threat Intel - Matched Target Email

## Description
Detects email addresses associated with known malicious actor(s) or campaign(s) as designated by a threat intelligence provider.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Threat Intelligence|
|Apply Risk to Entities|user_username, user_email, targetUser_username, targetUser_email|
|Signal Name|Threat Intel - Matched Target Email|
|Summary Expression|The record contains a target email address associated with a threat intelligence feed: {{targetUser_email}}|
|Score/Severity|Static: 1|
|Enabled by Default|True|
|Prototype|False|
|Tags||
## Vendors and Products
- [Google - G Suite](../products/e73cd65a-7a4b-4ce9-9d73-e5d9c824c214.md)
- [Microsoft - Azure](../products/a1225af5-e778-4068-a9a2-47da93d1ff24.md)
- [Proofpoint - Proofpoint on Demand](../products/332856e9-3111-446f-8df7-e64694e4b9a1.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|confidence|
|Normalized Schema|targetUser_email|
|Normalized Schema|targetUser_username|
|Normalized Schema|type|
|Normalized Schema|user_email|
|Normalized Schema|user_username|


