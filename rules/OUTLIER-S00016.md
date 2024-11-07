# [Rules](README.md): Okta - Outlier in OIDC token request failures

## Description
This signal looks for an outlier in the number of OpenID Connect (OIDC) token request failures for an Okta client application. Use the Okta admin portal to correlate the Client ID ( mapped to user_username ) to determine what application is being targeted. Pivot off the Client ID and IP address values to examine the raw Okta events in order to ensure that this activity is planned and expected. This activity can occur during setup and development of Okta applications and integrations.

## Additional Details
|Detail|Value|
|----|----|
|Type|Outlier|
|Category|Lateral Movement|
|Apply Risk to Entities|device_ip|
|Signal Name|Okta - Outlier in OIDC token request failures|
|Summary Expression|Okta - Outlier in OIDC token request failures from {{device_ip}} for the Client ID:  {{user_username}}|
|Retention Window|5184000000|
|Baseline Window|2592000000|
|Standard Deviation Threshold|1|
|Floor Value|1|
|Score/Severity|Static: 1|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0008, _mitreAttackTactic:TA0005, _mitreAttackTechnique:T1528|
## Vendors and Products
- [Okta - Single Sign-On](../products/51278354-d6b5-4c8e-a8fd-8197df334e67.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|device_ip|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_vendor|
|Normalized Schema|success|


