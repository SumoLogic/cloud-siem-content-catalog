# [Rules](README.md): Okta - Outlier in ASNs Used to Access Applications

## Description
This signal looks for an outlier in the number of distinct autonomous system numbers (ASNs) that a particular user utilizes to access Okta resources within an hour time period. This is designed to alert on various forms of token or credential theft as well as general Okta session anomalies.

## Additional Details
|Detail|Value|
|----|----|
|Type|Outlier|
|Category|Initial Access|
|Apply Risk to Entities|user_username|
|Signal Name|Okta - Outlier in ASNs Used to Access Applications by {{user_username}}|
|Summary Expression|Detected an outlier in the number of ASNs used to access Okta applications by {{user_username}}|
|Retention Window|1728000000|
|Baseline Window|1296000000|
|Standard Deviation Threshold|1|
|Floor Value|3|
|Score/Severity|Static: 2|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0001, _mitreAttackTechnique:T1078.004|
## Vendors and Products
- [Okta - Single Sign-On](../products/51278354-d6b5-4c8e-a8fd-8197df334e67.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_vendor|
|Normalized Schema|user_username|


