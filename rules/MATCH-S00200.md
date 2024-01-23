# [Rules](README.md): Potential Pass the Hash Activity

## Description
The behavior discovered here loosely matches the behavior of known pass the hash tools.  A Pass the Hash (PtH) attack is a way for an attacker to move laterally through a type of credential theft.  Because this behavior is known to occur in some environments during normal activity, tuning is recommended and attention paid to a possible spike in signals after enabling this rule.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Lateral Movement|
|Apply Risk to Entities|device_hostname, device_ip, user_username|
|Signal Name|Potential Pass the Hash Activity|
|Summary Expression|Potential pass the hash activity detected on host: {{device_hostname}}|
|Score/Severity|Static: 1|
|Enabled by Default|False|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0005, _mitreAttackTactic:TA0008, _mitreAttackTechnique:T1550, _mitreAttackTechnique:T1550.002|
## Vendors and Products
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|application|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Direct from Record|fields['EventData.KeyLength']|
|Normalized Schema|logonType|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|objectType|
|Normalized Schema|user_userId|
|Normalized Schema|user_username|


