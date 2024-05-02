# [Rules](README.md): Okta - Device Removed From User

## Description
An Okta device was removed from a user. It is recommended that the user performing the action be cross-referenced to a list of approved Okta administrators. In addition, examine the IP address of the user who is performing the action to determine of this activity is expected. The "target.1." fields of the detailed event contain information regarding which device was removed.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Persistence|
|Apply Risk to Entities|user_username|
|Signal Name|Okta - Device Removed From {{targetUser_username}}|
|Summary Expression|An Okta device was removed from the user: {{targetUser_username}} by {{user_username}} from the IP address of: {{srcDevice_ip}}|
|Score/Severity|Static: 1|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0003, _mitreAttackTactic:TA0004, _mitreAttackTechnique:T1098.005|
## Vendors and Products
- [Okta - Single Sign-On](../products/51278354-d6b5-4c8e-a8fd-8197df334e67.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_vendor|
|Normalized Schema|success|
|Normalized Schema|targetUser_username|
|Normalized Schema|user_username|


