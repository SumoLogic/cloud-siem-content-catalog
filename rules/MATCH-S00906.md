# [Rules](README.md): Okta - Application Created

## Description
This rule looks for an Okta application being created. Ensure that this activity is expected and authorized. Only Okta administrators should be creating applications. Check the Okta administrator portal for more details regarding the application in question such as scopes and access levels. The field "fields["target.1.alternateId"]" contains the name of the application that was created

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Defense Evasion|
|Apply Risk to Entities|user_username|
|Signal Name|Okta - Application Created|
|Summary Expression|An Okta application has been created by {{user_username}} from the IP address of {{device_ip}}|
|Score/Severity|Static: 2|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0005, _mitreAttackTactic:TA0008, _mitreAttackTechnique:T1550.001|
## Vendors and Products
- [Okta - Single Sign-On](../products/51278354-d6b5-4c8e-a8fd-8197df334e67.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_vendor|
|Normalized Schema|success|
|Normalized Schema|user_username|


