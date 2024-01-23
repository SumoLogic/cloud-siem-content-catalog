# [Rules](README.md): First Seen Kerberoasting Attempt from User - Host

## Description
First Seen Kerberos RC4 Request - If RC4 isn't used in the environment this indicates a possible Kerberoasting attempt.

## Additional Details
|Detail|Value|
|----|----|
|Type|First Seen|
|Category|Credential Access|
|Apply Risk to Entities|user_username, device_hostname|
|Signal Name|First Seen Kerberoasting Attempt from User on Host|
|Summary Expression|First Seen Kerberos RC4 Encryption Ticket Request|
|Retention Window|7776000000|
|Baseline Window|1209600000|
|Baseline Type|PER_ENTITY|
|Score/Severity|Static: 2|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0006, _mitreAttackTechnique:T1558, _mitreAttackTechnique:T1558.003|
## Vendors and Products
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|application|
|Normalized Schema|device_hostname|
|Normalized Schema|listMatches|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|resource|
|Normalized Schema|user_username|


