# [Rules](README.md): First Seen Weak Kerberos Encryption from User

## Description
Observes for first signs of Weak Kerberos Encryption from a User

## Additional Details
|Detail|Value|
|----|----|
|Type|First Seen|
|Category|Credential Access|
|Apply Risk to Entities|user_username|
|Signal Name|First Seen Weak Kerberos Encryption from User|
|Summary Expression|First Seen weak Kerberos Encryption seen for user: {{user_username}}|
|Retention Window|7776000000|
|Baseline Window|2592000000|
|Baseline Type|GLOBAL|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|True|
|Tags|_mitreAttackTactic:TA0006, _mitreAttackTechnique:T1558, _mitreAttackTechnique:T1558.003|
## Vendors and Products
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Direct from Record|fields["EventData.TicketEncryptionType"]|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|user_username|


