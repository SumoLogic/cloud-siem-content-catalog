# [Rules](README.md): Too Many Kerberos Encryption Downgrade SPNs (Kerberoasting)

## Description
Kerberoasting is an attack method that allows an attacker to crack the passwords of service accounts in Active Directory offline and without fear of detection. This is facilitated by requesting service tickets that have data encrypted with weak encryption types (typically RC4). This technique is described in https://attack.mitre.org/techniques/T1208/.

## Additional Details
|Detail|Value|
|----|----|
|Type|Threshold|
|Category|Credential Access|
|Apply Risk to Entities|user_username, srcDevice_ip|
|Signal Name|Too Many Kerberos Encryption Downgrade SPNs (Kerberoasting)|
|Summary Expression|Multiple Kerberos Encryption Downgrade SPNs from host {{srcDevice_ip}} in association with user {{user_username}}|
|Threshold Count|5|
|Threshold Window|5m|
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
|Direct from Record|fields['EventData.TicketEncryptionType']|
|Direct from Record|fields['EventData.TicketOptions']|
|Direct from Record|fields['insertionstrings_f05']|
|Direct from Record|fields['insertionstrings_f06']|
|Normalized Schema|listMatches|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|user_username|


