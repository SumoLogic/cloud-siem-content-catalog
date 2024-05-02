# [Rules](README.md): Okta - Device Added To User

## Description
An Okta device was added to a user. This activity may occur as part of normal user operations such as lost device. It is recommended that other events around this activity – particularly Okta events – be reviewed to determine if this activity is expected. The “target” element in the full event has the details of the type of device being added. This information can be used to confirm the activity with the user in question if deemed necessary.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Persistence|
|Apply Risk to Entities|user_username|
|Signal Name|Okta - Device Added To {{user_username}}|
|Summary Expression|An Okta device was added to the user: {{user_username}} with the IP address of: {{srcDevice_ip}}|
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
|Normalized Schema|user_username|


