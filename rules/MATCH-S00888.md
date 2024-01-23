# [Rules](README.md): Microsoft Teams External Access Enabled

## Description
Microsoft Teams External Access has been enabled, this settings allows any users that are external to your Teams/Office organization to message users that are within your Teams/Office organization. If this setting change is unplanned or unexpected it is recommended that this activity be reviewed.  MIcrosoft Teams provides administrators the ability to allow only specific external domains to message users within the organization. Look for Office 365 events with the "MessageSent" or "MemberAdded" event names in order to gain more detail as to what users were invited to which Teams channels - if any.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Initial Access|
|Apply Risk to Entities|device_ip|
|Signal Name|Microsoft Teams External Access Enabled by {{user_UserId}}|
|Summary Expression|Microsoft Team External Access has been enabled by {{user_UserId}}|
|Score/Severity|Static: 4|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0001, _mitreAttackTechnique:T1566|
## Vendors and Products
- [Microsoft - Office 365](../products/d3ed003d-5ddd-4c7a-bea5-63eae6311833.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|action|
|Normalized Schema|device_ip|
|Direct from Record|fields["ModifiedProperties.1.Name"]|
|Direct from Record|fields["ModifiedProperties.1.NewValue"]|
|Normalized Schema|metadata_product|
|Normalized Schema|user_UserId|


