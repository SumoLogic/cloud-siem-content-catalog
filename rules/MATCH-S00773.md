# [Rules](README.md): Salesforce LoginAs Event

## Description
Generates severity 0 signals for LoginAs Salesforce events. The purpose of this rule is to track LoginAs activity for both the source and target user to provide additional context for Insights. The third party match list exclusion should be populated to exclude known permitted third party domains from triggering this rule. Its common for third party support accounts to use the LoginAs function. Salesforce admin match lists are exclude in this rule in an attempt to reduce the false positives due to expected admin activity. These match lists should be created and populated with Salesforce admin usernames and IPs.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Credential Access|
|Apply Risk to Entities|srcDevice_ip, user_username, targetUser_username|
|Signal Name|Salesforce LoginAs Event|
|Summary Expression|Salesforce LoginAs Event from Source User: {{user_username}} IP: {{srcDevice_ip}} to Target User: {{targetUser_username}}|
|Score/Severity|Static: 0|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0006, _mitreAttackTechnique:T1078.004, _mitreAttackTechnique:T1078|
## Vendors and Products


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|listMatches|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|targetUser_username|
|Normalized Schema|user_username|


