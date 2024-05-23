# [Rules](README.md): Okta - Session Anomaly (Multiple User Agents)

## Description
This rule detects when a user has utilized multiple distinct User Agents when performing authentication through Okta. This activity could potentially indicate credential theft or a general session anomaly. Examine other Okta related events surrounding the time period for this signal, pivoting off the username value to examine if any other suspicious activity has taken place. If this rule is generating false positives, adjust the threshold value and consider excluding certain user accounts via tuning expression.

## Additional Details
|Detail|Value|
|----|----|
|Type|Aggregation|
|Category|Initial Access|
|Apply Risk to Entities|user_username|
|Signal Name|Okta - Session Anomaly (Multiple User Agents) for user: {{user_username}}|
|Summary Expression|{{user_username}} has utilized a number of distinct User Agents which has crossed the threshold (4) value within a 30-minute time period to perform Okta authentication.|
|Aggregation Window|T30M|
|Score/Severity|Static: 1|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0001, _mitreAttackTechnique:T1078.004|
## Vendors and Products
- [Okta - Single Sign-On](../products/51278354-d6b5-4c8e-a8fd-8197df334e67.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|distinct_userAgents|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_vendor|
|Normalized Schema|user_username|


