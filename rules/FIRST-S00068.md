# [Rules](README.md): Okta - First Seen User Accessing Admin Application

## Description
A user not seen since the baseline period has accessed the Okta admin application. Ensure that this user is expected to perform Okta administrative activities. If this user is expected and authroized, consider adding the user to the "Okta_Admins" match list to exclude the user from this signal.

## Additional Details
|Detail|Value|
|----|----|
|Type|First Seen|
|Category|Initial Access|
|Apply Risk to Entities|user_username|
|Signal Name|Okta - First Seen User:{{user_username}}  has successfully accessed the Okta Admin Application|
|Summary Expression|First Seen User ( {{user_username}} )  Accessing Okta Admin Application|
|Retention Window|7776000000|
|Baseline Window|2592000000|
|Baseline Type|GLOBAL|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0001, _mitreAttackTactic:TA0004, _mitreAttackTechnique:T1552, _mitreAttackTechnique:T1552.005, _mitreAttackTechnique:T1078.004|
## Vendors and Products
- [Okta - Single Sign-On](../products/51278354-d6b5-4c8e-a8fd-8197df334e67.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|listMatches|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_vendor|
|Normalized Schema|success|
|Normalized Schema|user_username|


