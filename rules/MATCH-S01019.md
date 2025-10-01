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
- [Microsoft - Azure](../products/a1225af5-e778-4068-a9a2-47da93d1ff24.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|confidence|
|Normalized Schema|targetUser_email|
|Normalized Schema|targetUser_username|
|Normalized Schema|type|
|Normalized Schema|user_email|
|Normalized Schema|user_username|


