# [Rules](README.md): Okta - Outlier in MFA Attempts Denied by User

## Description
This signal builds an hourly baseline of MFA denied events per user and triggers when an outlier in the number of denied attempts is detected. This signal is designed to trigger on MFA-fatigue type attacks. If false positives are detected, consider excluding certain users from the alerting logic or raise the minimum count value within the rule configuration.

## Additional Details
|Detail|Value|
|----|----|
|Type|Outlier|
|Category|Credential Access|
|Apply Risk to Entities|user_username|
|Signal Name|Okta - Outlier in MFA Attempts Denied by {{user_username}}|
|Summary Expression|Outlier in Okta MFA Attempts Denied by {{user_username}} from {{srcDevice_ip}}|
|Retention Window|345600000|
|Baseline Window|259200000|
|Standard Deviation Threshold|1|
|Floor Value|1|
|Score/Severity|Static: 2|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0006, _mitreAttackTechnique:T1621|
## Vendors and Products
- [Okta - Single Sign-On](../products/51278354-d6b5-4c8e-a8fd-8197df334e67.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|description|
|Direct from Record|fields["debugContext.debugData.pushOnlyResponseType"]|
|Normalized Schema|metadata_vendor|
|Normalized Schema|user_username|


