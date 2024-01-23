# [Rules](README.md): Salesforce Permission Set Assigned

## Description
Detects permission set assignments. While this is a routine activity, permission assignments could be used by an adversary for persistence and privilege escalation. Salesforce admin match lists are exclude in this rule in an attempt to reduce the false positives due to expected admin activity. These match lists should be created and populated with Salesforce admin usernames and IPs.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Persistence|
|Apply Risk to Entities|srcDevice_ip, user_username|
|Signal Name|Salesforce Permission Set Assigned|
|Summary Expression|Salesforce Permission Set Assigned: {{description}} User: {{user_username}} IP: {{srcDevice_ip}}|
|Score/Severity|Dynamic: 1 or 2|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0003, _mitreAttackTechnique:T1098|
## Vendors and Products


## Dynamic Signal Score/Severity Translation

The default score of `1` is used as a catch all if none of the translations are met.

|Schema Field|Field Value|Score/Severity|
|------------|-----------|--------------|
|metadata_deviceEventId|PermSetLicenseAssign|2|
## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|listMatches|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|user_username|


