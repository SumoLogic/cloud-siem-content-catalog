# [Rules](README.md): Salesforce WaveDownload Event

## Description
Wave Download events represent downloads made from lens explorations and dashboard widgets in the Tableau CRM user interface. A Wave Download event type is captured when a user downloads images ( .png ), Microsoft Excel data ( .xls ), or comma-separated values ( .csv ) files. Salesforce admin match lists are exclude in this rule in an attempt to reduce the false positives due to expected admin activity. These match lists should be created and populated with Salesforce admin usernames and IPs.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Collection|
|Apply Risk to Entities|srcDevice_ip, user_username|
|Signal Name|Salesforce WaveDownload Event|
|Summary Expression|Salesforce WaveDownload Event: {{description}} with User: {{user_username}} IP: {{srcDevice_ip}}|
|Score/Severity|Static: 2|
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


