# [Rules](README.md): Okta - MFA Request Denied by User

## Description
This signal will trigger when a user denies an MFA request within the Okta authenticator application. Examine other authentication attempts for this particular user and undertake confirmation efforts to ensure that  this activity is expected and valid.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Initial Access|
|Apply Risk to Entities|user_username|
|Signal Name|Okta - MFA Request Denied by {{user_username}}|
|Summary Expression|An Okta MFA Request/Prompt was Denied by {{user_username}}|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0001, _mitreAttackTechnique:T1078.004|
## Vendors and Products
- [Okta - Single Sign-On](../products/51278354-d6b5-4c8e-a8fd-8197df334e67.md)


## Fields Used

|Origin|Field|
|----|----|
|Direct from Record|fields["debugContext.debugData.pushOnlyResponseType"]|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_vendor|
|Normalized Schema|user_username|


