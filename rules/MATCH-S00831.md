# [Rules](README.md): Office 365 Unified Audit Logging Disabled

## Description
Cloud environments such as Office 365 and Azure allow for collection and analysis of audit telemetry that provides insight into what activities a user does within the Office 365 environment. If a threat actor has sufficient permissions, they can disable logging to avoid detection of their potentially malicious activities.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Defense Evasion|
|Apply Risk to Entities|user_username|
|Signal Name|{{user_username}} has turned off Unified Audit Logging in Office 365|
|Summary Expression|The Office 365 Unified Audit Log logs Office 365 and Azure Active Directory activites including sign ins, Teams activity, SharePoint activity and OneDrive activity. Unplanned and unexpected occurances of this event should be investigated.|
|Score/Severity|Static: 6|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0005, _mitreAttackTechnique:T1562.008|
## Vendors and Products
- [Microsoft - Office 365](../products/d3ed003d-5ddd-4c7a-bea5-63eae6311833.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|action|
|Direct from Record|fields["UnifiedAuditLogIngestionEnabled"]|
|Normalized Schema|metadata_product|
|Normalized Schema|user_username|


