# [Rules](README.md): Salesforce Excessive Documents Downloaded

## Description
Detects when an entity downloads multiple documents or attachments in a short timeframe. This type of activity is indicative of exfiltration. Salesforce admin match lists are exclude in this rule in an attempt to reduce the false positives due to expected admin activity. These match lists should be created and populated with Salesforce admin usernames and IPs.

## Additional Details
|Detail|Value|
|----|----|
|Type|Threshold|
|Category|Collection|
|Apply Risk to Entities|srcDevice_ip, user_username|
|Signal Name|Salesforce Excessive Documents Downloaded|
|Summary Expression|Salesforce Excessive Documents Downloaded from User: {{user_username}} IP: {{srcDevice_ip}}|
|Threshold Count|5|
|Threshold Window|5m|
|Score/Severity|Static: 1|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0009, _mitreAttackTechnique:T1213, _mitreAttackTechnique:T1530|
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


