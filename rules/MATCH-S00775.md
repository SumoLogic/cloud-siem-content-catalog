# [Rules](README.md): Salesforce User Creation

## Description
Detects user creation. While this is a routine activity, user creation could be used by an adversary for persistence. Salesforce admin match lists are exclude in this rule in an attempt to reduce the false positives due to expected admin activity. These match lists should be created and populated with Salesforce admin usernames and IPs.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Persistence|
|Apply Risk to Entities|srcDevice_ip, user_username|
|Signal Name|Salesforce User Creation|
|Summary Expression|{{description}}|
|Score/Severity|Static: 1|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0003, _mitreAttackTechnique:T1136, _mitreAttackTechnique:T1136.003|
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


