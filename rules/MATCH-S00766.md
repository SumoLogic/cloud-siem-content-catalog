# [Rules](README.md): Okta MFA Deactivated for User

## Description
This rule detects multi-factor authentication (MFA) being disabled for a user. An adversary or malicious insider may deactivate MFA in order to bypass security controls. The Okta_Admins match list should be created and populated with administrator users permitted to perform this activity.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Credential Access|
|Apply Risk to Entities|user_username, srcDevice_ip, targetUser_username|
|Signal Name|Okta MFA Deactivated for User|
|Summary Expression|MFA deactivated for user {{targetUser_username}}|
|Score/Severity|Static: 5|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0006, _mitreAttackTechnique:T1111|
## Vendors and Products
- [Okta - Single Sign-On](../products/51278354-d6b5-4c8e-a8fd-8197df334e67.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|listMatches|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|targetUser_username|
|Normalized Schema|user_username|


