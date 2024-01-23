# [Rules](README.md): Blocked Email Message

## Description
An SMTP server sent a reply mentioning an SMTP block list.

## Additional Details
|Detail|Value|
|----|----|
|Type|Match|
|Category|Initial Access|
|Apply Risk to Entities|srcDevice_ip|
|Signal Name|Blocked Email Message|
|Summary Expression|Blocked Email message from {{srcDevice_ip}}|
|Score/Severity|Static: 2|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0001, _mitreAttackTactic:TA0043, _mitreAttackTechnique:T1566, _mitreAttackTechnique:T1566.001, _mitreAttackTechnique:T1566.002, _mitreAttackTechnique:T1598, _mitreAttackTechnique:T1598.002, _mitreAttackTechnique:T1598.003|
## Vendors and Products
- [Bro - Bro](../products/37C866BF-72E1-470A-9072-EDB908F56951.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_product|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|threat_name|


