# [Rules](README.md): Claude Compliance API Logging Disabled

## Description
Detection:
This rule triggers when an administrator disables Compliance API activity logging for the organization.

Scenario:
An attacker with administrative access may disable Compliance API logging to cover their tracks before performing data exfiltration or other malicious activities. Disabling this logging removes the organization's ability to monitor API access patterns via the Activity Feed, creating a blind spot in security monitoring. The Compliance API provides access to organizational chats, files, and projects, making unmonitored access a significant data loss risk.

Recommended Actions:
Verify with the organization's security team whether this change was authorized and re-enable compliance API logging if not. Review recent activity from user_username for signs of compromise and audit any Compliance API activity that occurred while logging was disabled.

Tuning Recommendations:
This rule should have a low false positive rate as disabling compliance logging is a rare and significant security control change. Consider creating a match list of authorized administrators who manage compliance settings during scheduled maintenance windows.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Defense Evasion|
|Apply Risk to Entities|user_username|
|Signal Name|Claude Compliance API Logging Disabled by {{user_username}}|
|Summary Expression|Claude Compliance API Logging Disabled by {{user_username}} from IP {{device_ip}}|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0112, _mitreAttackTechnique:T1685.002, _mitreAtlasTactic:AML.TA0007|
## Vendors and Products
- [Anthropic - Claude Activity Logs](../products/8ad9c55c-1271-4e8a-a8ca-f1663051f4d1.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|action|
|Direct from Record|fields.compliance_api_logging_enabled|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|user_username|


