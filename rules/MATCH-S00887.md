# [Rules](README.md): Port Forwarding Enabled via Visual Studio Code

## Description
A local port has been forwarded and made available for external connectivity utilizing the Visual Studio Code port forwarding feature. Ensure that this activity is expected and approved, as it may be used by developers for legitimate purposes. This activity could potentially circumvent existing egress/ingress controls by exposing local services to the internet. Look for other events around this time frame in order to ascertain the purpose for the port forwarding activities. If tuning of the rule is required, create a list that contains developers who utilize this functionality and exclude it from the expression.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Command and Control|
|Apply Risk to Entities|user_username|
|Signal Name|Port Forwarding Enabled via Visual Studio Code on {{device_hostname}} by {{user_username}}|
|Summary Expression|Port Forwarding Enabled via Visual Studio Code on {{device_hostname}} by {{user_username}}|
|Score/Severity|Static: 1|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0011, _mitreAttackTechnique:T1572|
## Vendors and Products
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|device_hostname|
|Normalized Schema|objectClassification|
|Normalized Schema|user_username|


