# [Rules](README.md): Proofpoint TAP - IP Sent Impostor Email

## Description
Proofpoint TAP detected an IP address sending an email with an impostor score 75 or higher. Records indicating the email was permitted will have a higher signal score compared to those automatically blocked by Proofpoint.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Initial Access|
|Apply Risk to Entities|srcDevice_ip|
|Signal Name|Proofpoint TAP - IP Sent Impostor Email|
|Summary Expression|Imposter from IP: {{srcDevice_ip}} {{action}} on IP: {{device_ip}} by user: {{user_username}}|
|Score/Severity|Dynamic: 1 or 3|
|Enabled by Default|False|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0001, _mitreAttackTactic:TA0009, _mitreAttackTactic:TA0043, _mitreAttackTechnique:T1566, _mitreAttackTechnique:T1566.001, _mitreAttackTechnique:T1566.002, _mitreAttackTechnique:T1598, _mitreAttackTechnique:T1598.002, _mitreAttackTechnique:T1598.003|
## Vendors and Products
- [Proofpoint - Targeted Attack Protection](../products/de3d4b6b-36a3-4436-8bfc-0561ac95037e.md)


## Dynamic Signal Score/Severity Translation

The default score of `1` is used as a catch all if none of the translations are met.

|Schema Field|Field Value|Score/Severity|
|------------|-----------|--------------|
|metadata_deviceEventId|MESSAGE_BLOCKED|1|
|metadata_deviceEventId|MESSAGE_PERMITTED|3|
|metadata_deviceEventId|MESSAGE_DELIVERED|3|
## Fields Used

|Origin|Field|
|----|----|
|Direct from Record|fields['impostorScore']|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|srcDevice_ip|


