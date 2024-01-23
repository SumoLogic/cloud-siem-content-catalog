# [Rules](README.md): Okta MFA Bypass Attempt

## Description
Attempts to bypass MFA can be indicative of malicious actors having compromised the password for an account but not the corresponding MFA token and such attempts should be audited for legitimacy.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Credential Access|
|Apply Risk to Entities|user_username, srcDevice_ip|
|Signal Name|Okta MFA Bypass Attempt|
|Summary Expression|MFA bypass attempt for user {{user_username}} from ip {{srcDevice_ip}}|
|Score/Severity|Static: 4|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0006, _mitreAttackTechnique:T1111|
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


