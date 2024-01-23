# [Rules](README.md): First Seen Azure Device Code Authentication from User

## Description
Azure Device Code authentication can be utilized in phishing attacks. This specific rule looks for a user performing device code authentication to an Azure resource for the first time since the baseline period. If this action is not expected, it could be a sign of malicious activity. Examine the event for odd user agent values and look at what other actions the affected account is performing within the Azure estate.

## Additional Details
|Detail|Value|
|----|----|
|Type|First Seen|
|Category|Initial Access|
|Apply Risk to Entities|user_username|
|Signal Name|First Seen Azure Device Code Authentication from User|
|Summary Expression|First Seen Azure Device Code Authentication from {{user_username}}|
|Retention Window|5184000000|
|Baseline Window|1209600000|
|Baseline Type|GLOBAL|
|Score/Severity|Static: 6|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0001, _mitreAttackTactic:TA0007, _mitreAttackTechnique:T1078.004, _mitreAttackTechnique:T1098|
## Vendors and Products
- [Microsoft - Azure](../products/a1225af5-e778-4068-a9a2-47da93d1ff24.md)


## Fields Used

|Origin|Field|
|----|----|
|Direct from Record|fields['properties.authenticationProtocol']|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|user_username|


