# [Rules](README.md): Okta - MFA Denied Followed by Successful Logon

## Description
This signal looks for a single user explicitly denying at least two (2) multi factor authentication prompts, followed by a successful Okta login via multi factor authentication within a twenty-five (25) minute window. This logic is designed to catch successful MFA fatigue type attacks. If you find this signal is triggering on legitimate events, consider excluding certain users via tuning expressions. You can also consider tweaking the time window within the "Grouped by" portion of the rule. 

## Additional Details
|Detail|Value|
|----|----|
|Type|Chain|
|Category|Credential Access|
|Apply Risk to Entities|user_username|
|Signal Name|Okta - MFA Denied Followed by Successful Logon|
|Summary Expression|Okta - MFA Denied Followed by Successful Logon for: {{user_username}}|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0006, _mitreAttackTechnique:T1621|
## Vendors and Products
- [Okta - Single Sign-On](../products/51278354-d6b5-4c8e-a8fd-8197df334e67.md)


## Fields Used

|Origin|Field|
|----|----|
|Direct from Record|fields["debugContext.debugData.pushOnlyResponseType"]|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_vendor|
|Normalized Schema|success|
|Normalized Schema|user_username|


