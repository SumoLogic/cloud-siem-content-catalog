# [Rules](README.md): First Seen User Initiating Claude Data Export

## Description
Detection:
This rule triggers the first time a user initiates a Claude organization data export within a 90-day baseline window.

Scenario:
An attacker with administrative access may initiate a large-scale data export to exfiltrate organizational data including chat histories, files, and project information. Data exports are powerful bulk operations that can expose sensitive intellectual property, customer data, or strategic information in a single action.

Recommended Actions:
Verify the data export was authorized by confirming user_username has a legitimate business need (e.g., legal hold, compliance audit, offboarding). If unauthorized, revoke the user's access and investigate whether the export file was accessed or downloaded.

Tuning Recommendations:
Organizations that perform regular scheduled exports for compliance purposes should baseline those service accounts. Create a match list of accounts authorized to perform data exports to reduce noise from legitimate operations.

## Additional Details
|Detail|Value|
|----|----|
|Type|First Seen|
|Category|Collection|
|Apply Risk to Entities|user_username|
|Signal Name|User {{user_username}} Initiated Claude Data Export for the First Time|
|Summary Expression|User {{user_username}} initiated Claude data export for the first time since baseline|
|Retention Window|7776000000|
|Baseline Window|0|
|Baseline Type|GLOBAL|
|Score/Severity|Static: 4|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0009, _mitreAttackTechnique:T1567, _mitreAtlasTactic:AML.TA0010, _mitreAtlasTechnique:AML.T0025, _mitreAtlasTechnique:AML.T0048.004|
## Vendors and Products


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|action|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|user_username|


