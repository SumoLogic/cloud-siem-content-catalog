# [Rules](README.md): Okta - Policy Rule Added

## Description
An Okta policy rule has been added through the Okta admin application. The field "fields["target.1.displayName"]" contains the name of this rule for investigation purposes. Ensure that this activity is planned and performed by an authorized Okta administrator. Examine other generated signals for the user to further investigation activities.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Initial Access|
|Apply Risk to Entities|user_username, srcDevice_ip|
|Signal Name|Okta - Policy Rule Added|
|Summary Expression|Okta Policy Rule Added by {{user_username}} from {{srcDevice_ip}}|
|Score/Severity|Static: 2|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0001, _mitreAttackTechnique:T1078.004|
## Vendors and Products
- [Okta - Single Sign-On](../products/51278354-d6b5-4c8e-a8fd-8197df334e67.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|description|
|Normalized Schema|metadata_vendor|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|user_username|


