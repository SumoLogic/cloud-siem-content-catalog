# [Rules](README.md): Azure DevOps - New Extension Installed

## Description
Context:
Azure DevOps can add extensions for additional features. Attackers with sufficient privileges may install a malicious extension for malicious use. 

Detection:
This detection monitors for new extensions installed organization-wide after a 30-day baseline, based on the user installing the new extension.

Recommended Actions: 
As new extensions are installed, investigate the user engaging in the activity to assess the intent. Review whether the user has been active and engaged in other suspicious activity.  

Tuning Recommendations:
Add a tuning expression with user_username values or a match list for users known and trusted to install extensions. 
A tuning expression of permitted PublisherName values can be used to add further filtering. You may want to increase the severity of this rule if your organization only permits certain PublisherNames.
 
Credits:
This detection is based on the Azure Sentinel ADONewExtensionAdded.yaml rule.

## Additional Details
|Detail|Value|
|----|----|
|Type|First Seen|
|Category|Persistence|
|Apply Risk to Entities|user_username|
|Signal Name|Azure DevOps - First Seen New Extension Installed|
|Summary Expression|User: {{user_username}} has installed a new Azure DevOps Extension|
|Retention Window|7776000000|
|Baseline Window|2592000000|
|Baseline Type|GLOBAL|
|Score/Severity|Static: 2|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTechnique:T1505, _mitreAttackTactic:TA0003|
## Vendors and Products
- [Microsoft - Azure DevOps Auditing](../products/c3b61ddb-4d2d-497c-b873-28938036b67b.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|action|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|user_username|


