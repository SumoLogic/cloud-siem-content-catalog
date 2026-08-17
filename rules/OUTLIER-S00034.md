# [Rules](README.md): Outlier in Claude Compliance API Calls from User

## Description
Detection:
This rule triggers when the number of Compliance API calls from a single user in a one-hour window exceeds the established baseline by 2 standard deviations with a minimum floor of 15 calls.

Scenario:
An attacker who has compromised Compliance API credentials may perform automated bulk data retrieval, scraping chat contents, files, and organizational data at a rate significantly above normal usage patterns. Elevated API call volumes may indicate reconnaissance or bulk data exfiltration via the Compliance API's access to chats, files, projects, and user data.

Recommended Actions:
Review the URLs and request methods for the user to determine what data was being accessed, and verify whether the spike correlates with a legitimate bulk operation (e.g., scheduled SIEM ingestion or eDiscovery export). If unauthorized, rotate the Compliance Access Key immediately and audit what data was retrieved during the anomalous period.

Tuning Recommendations:
Adjust the floor_value based on your organization's normal Compliance API usage patterns. Organizations with automated SIEM pipelines or scheduled eDiscovery jobs should baseline those service accounts separately or exclude them via match list.

## Additional Details
|Detail|Value|
|----|----|
|Type|Outlier|
|Category|Collection|
|Apply Risk to Entities|user_username|
|Signal Name|Outlier in Claude Compliance API Calls from User: {{user_username}}|
|Summary Expression|User {{user_username}} generated an unusual number of Compliance API calls in a one-hour window, exceeding the 30-day baseline by more than 2 standard deviations|
|Retention Window|7776000000|
|Baseline Window|2592000000|
|Standard Deviation Threshold|2|
|Floor Value|15|
|Score/Severity|Static: 2|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0009, _mitreAttackTechnique:T1530, _mitreAtlasTactic:AML.TA0009, _mitreAtlasTechnique:AML.T0085, _mitreAtlasTechnique:AML.T0096|
## Vendors and Products


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|action|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|user_username|


