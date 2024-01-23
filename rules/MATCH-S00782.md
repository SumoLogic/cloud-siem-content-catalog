# [Rules](README.md): Salesforce Permission Set Deletion

## Description
Detects permission set deletions in Salesforce. While these deletions can be routine, their function can be abused for malicious intent. Salesforce admin match lists are exclude in this rule in an attempt to reduce the false positives due to expected admin activity. These match lists should be created and populated with Salesforce admin usernames and IPs.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Persistence|
|Apply Risk to Entities|srcDevice_ip, user_username|
|Signal Name|Salesforce Permission Set Deletion|
|Summary Expression|Salesforce Permission Set Deletion: {{description}} User: {{user_username}} IP: {{srcDevice_ip}}|
|Score/Severity|Static: 1|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0003, _mitreAttackTechnique:T1098, _mitreAttackTactic:TA0040, _mitreAttackTechnique:T1485, _mitreAttackTechnique:T1531|
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


