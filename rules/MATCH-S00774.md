# [Rules](README.md): Salesforce Custom Permission Creation

## Description
Custom Permissions in Salesforce are used to give access to users for certain apps or processes that you have configured and which cannot be controlled by profile or permission set directly. This rule is used to monitor this activity as adversaries could abuse this to escalate privileges. Salesforce admin match lists are exclude in this rule in an attempt to reduce the false positives due to expected admin activity. These match lists should be created and populated with Salesforce admin usernames and IPs.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Persistence|
|Apply Risk to Entities|srcDevice_ip, user_username|
|Signal Name|Salesforce Custom Permission Creation|
|Summary Expression|Salesforce Custom Permission Creation: {{description}} with User: {{user_username}} IP: {{srcDevice_ip}}|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0003, _mitreAttackTechnique:T1098, _mitreAttackTechnique:T1098.001|
## Vendors and Products


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|listMatches|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|user_username|


