# [Rules](README.md): Outlier in Claude Resource Deletions from User

## Description
Detection:
This rule triggers when the number of Claude resource deletions (chats, projects, and files) from a single user in a one-hour window exceeds the established baseline by 2 standard deviations with a minimum floor of 5 deletions.

Scenario:
An attacker or malicious insider may perform mass deletions of chats, projects, and files to destroy evidence of unauthorized activity, sabotage organizational resources, or cause operational disruption. A sudden spike in deletions from a single user is anomalous and may indicate account compromise or insider threat activity. Content deleted by users is permanently removed and not recoverable via the Compliance API.

Recommended Actions:
Review other recent activity from user_username for signs of account compromise and determine if the deletions align with an authorized cleanup or offboarding process. If unauthorized, suspend the user's access immediately — deleted content cannot be recovered, so timely response is critical.

Tuning Recommendations:
Adjust the floor_value based on your organization's normal deletion patterns. Users performing authorized bulk cleanup (e.g., departing employees with IT oversight, periodic project archival) can be temporarily excluded via match list during approved operations.

## Additional Details
|Detail|Value|
|----|----|
|Type|Outlier|
|Category|Impact|
|Apply Risk to Entities|user_username|
|Signal Name|Outlier in Claude Resource Deletions from User: {{user_username}}|
|Summary Expression|User {{user_username}} performed an unusual number of Claude resource deletions (chats, projects, or files) in a one-hour window, exceeding the 30-day baseline by more than 2 standard deviations|
|Retention Window|7776000000|
|Baseline Window|2592000000|
|Standard Deviation Threshold|2|
|Floor Value|5|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0040, _mitreAttackTechnique:T1485, _mitreAtlasTactic:AML.TA0011, _mitreAtlasTechnique:AML.T0029, _mitreAtlasTechnique:AML.T0101|
## Vendors and Products
- [Anthropic - Claude Activity Logs](../products/8ad9c55c-1271-4e8a-a8ca-f1663051f4d1.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|action|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|user_username|


