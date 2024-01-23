# [Rules](README.md): Okta Account Primary Email Address Update

## Description
An Okta accounts primary email address has been updated. An adversary may modify an Okta accounts email address to evade detection by users or to gather information about the organization and establish persistence through credential resets.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Collection|
|Apply Risk to Entities|user_username, srcDevice_ip|
|Signal Name|Okta Account Primary Email Address Update|
|Summary Expression|Primary email address changed for user {{user_username}}|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0009, _mitreAttackTechnique:T1114.002, _mitreAttackTactic:TA0003, _mitreAttackTechnique:T1098|
## Vendors and Products
- [Okta - Single Sign-On](../products/51278354-d6b5-4c8e-a8fd-8197df334e67.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|user_username|


