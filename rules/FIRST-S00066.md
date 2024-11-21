# [Rules](README.md): Okta - First Seen User Requesting Report

## Description
This signal looks for a first seen user requesting an export of an Okta report. The various Okta report types can be found in the “Reports” section of the Okta administrative portal and can include various report types such as application password help, MFA usage and reports around user access. During the October 2023 Okta incident, threat actors downloaded reports from Okta portals to extract information regarding user contact information. Ensure that the user that is requesting such reports is authorized and that this activity is expected. If a suspicious report generation event occurs, look at the “target” element within the event to gain more detailed information as to the type of report being generated and exported.

## Additional Details
|Detail|Value|
|----|----|
|Type|First Seen|
|Category|Discovery|
|Apply Risk to Entities|user_username|
|Signal Name|First Seen user: {{user_username}} requesting Okta report|
|Summary Expression|First Seen user: {{user_username}} requesting Okta report from IP address: {{srcDevice_ip}}|
|Retention Window|7776000000|
|Baseline Window|2592000000|
|Baseline Type|GLOBAL|
|Score/Severity|Static: 2|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0007, _mitreAttackTechnique:T1087.004|
## Vendors and Products
- [Okta - Single Sign-On](../products/51278354-d6b5-4c8e-a8fd-8197df334e67.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_vendor|
|Normalized Schema|user_username|


