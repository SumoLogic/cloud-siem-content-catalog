# [Rules](README.md): Microsoft Teams Guest Access Enabled

## Description
Microsoft Teams Guest Access has been enabled globally, this settings allows any users that are external to your Teams/Office organization to be invited into your Teams/Office organization. If this setting change is unplanned or unexpected it is recommended that this activity be reviewed. MIcrosoft Teams provides administrators the ability to allow only specific guest actions to take place within the Teams/Office organization.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Initial Access|
|Apply Risk to Entities|device_ip|
|Signal Name|Microsoft Teams Guest Access Enabled by {{user_userId}}|
|Summary Expression|Microsoft Team Guest Access has been enabled by {{user_userId}}|
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
|Normalized Schema|user_userId|


