# [Rules](README.md): Kerberos Manipulation

## Description
This method triggers on rare Kerberos Failure Codes caused by manipulations of Kerberos messages.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Credential Access|
|Apply Risk to Entities|device_ip, user_username|
|Signal Name|Kerberos Manipulation|
|Summary Expression|Possible Kerberos manipulation on host: {{device_hostname}}|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0006, _mitreAttackTechnique:T1212|
## Vendors and Products
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|device_ip|
|Normalized Schema|errorCode|
|Direct from Record|fields['insertionstrings_f05']|
|Direct from Record|fields['insertionstrings_f07']|
|Direct from Record|fields['insertionstrings_f09']|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|user_username|


