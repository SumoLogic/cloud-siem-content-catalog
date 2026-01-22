# [Rules](README.md): Salesforce Report Exported

## Description
Detects when a report is exported. Reports contain a variety of information that adversaries may attempt to exfiltrate. Salesforce admin match lists are exclude in this rule in an attempt to reduce the false positives due to expected admin activity. These match lists should be created and populated with Salesforce admin usernames and IPs.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Collection|
|Apply Risk to Entities|srcDevice_ip, user_username|
|Signal Name|Salesforce Report Exported|
|Summary Expression|Salesforce Report Exported with User: {{user_username}} IP: {{srcDevice_ip}}|
|Score/Severity|Static: 2|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0009, _mitreAttackTechnique:T1213, _mitreAttackTechnique:T1530|
## Vendors and Products
- [Salesforce - Salesforce](../products/1b7798df-963b-4582-a82b-b8176c3a6a22.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|user_username|


