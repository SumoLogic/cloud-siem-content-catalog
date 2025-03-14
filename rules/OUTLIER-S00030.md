# [Rules](README.md): Azure DevOps - Outlier in Pools Deleted Rapidly

## Description
Context:
An Attacker with sufficient administrative access to Azure DevOps (ADO) may abuse this access to destroy existing resources by deleting pools. 

Detection:
This detection identifies statistical outliers in user behavior for the number of pools deleted in an hourly window. 

Recommended Actions: 
If an alert occurs, investigate the actions taken by the account to determine if this is normal operation of deleting pools or if this suspicious activity. 

Tuning Recommendations:
Determine if the baseline basis should be hourly or daily based on normal activity in your organization. 
If the detection is proving to be too sensitive to the number of pools deleted, adjust the floor value (currently 3) to a number that is less sensitive but within reason. Use Sumo Search using a count and the _timeslice function to aggregate on the number of pools deleted within the hourly (or daily) periods to find what is an acceptable level of activity to not alert on.

## Additional Details
|Detail|Value|
|----|----|
|Type|Outlier|
|Category|Defense Evasion|
|Apply Risk to Entities|user_username|
|Signal Name|Azure DevOps - Outlier in Agent Pools Deleted in an Hour|
|Summary Expression|User: {{user_username}} has deleted an abnormal amount of Agent Pools within an hour|
|Retention Window|7776000000|
|Baseline Window|2592000000|
|Standard Deviation Threshold|3|
|Floor Value|3|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTechnique:T1578.002, _mitreAttackTactic:TA0005|
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


