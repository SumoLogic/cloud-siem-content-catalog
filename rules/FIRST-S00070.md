# [Rules](README.md): Okta - First Seen Application Accessed by User

## Description
This signal looks for a user that is accessing an application behind Okta SSO that is first seen since the baseline period. Ensure that access of this application is expected and authorized, look for other Okta events around the user account in question to determine whether access to this application is expected and authorized.

## Additional Details
|Detail|Value|
|----|----|
|Type|First Seen|
|Category|Initial Access|
|Apply Risk to Entities|user_username|
|Signal Name|Okta - First Seen Application Accessed by {{user_username}}|
|Summary Expression|{{user_username}} has an accessed an Okta application not seen since the baseline period.|
|Retention Window|3024000000|
|Baseline Window|2592000000|
|Baseline Type|PER_ENTITY|
|Score/Severity|Static: 1|
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


