# [Rules](README.md): Windows - Excessive User Interactive Logons Across Multiple Hosts

## Description
A user performed a significant number of Windows interactive logins to multiple destination hosts in the past 24 hours. This behavior can be expected for some accounts, such as administrators in a Windows environment. Tuning this rule is highly recommended to filter out usernames where applicable.

## Additional Details
|Detail|Value|
|----|----|
|Type|Threshold|
|Category|Lateral Movement|
|Apply Risk to Entities|user_username|
|Signal Name|Windows - Excessive User Interactive Logons Across Multiple Hosts|
|Summary Expression|The account {{user_username}}  was observed interactively logging into 10+ unique destination hosts within the past 24 hours.|
|Threshold Count|10|
|Threshold Window|24h|
|Score/Severity|Static: 1|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0001, _mitreAttackTactic:TA0003, _mitreAttackTactic:TA0004, _mitreAttackTactic:TA0005, _mitreAttackTactic:TA0008, _mitreAttackTechnique:T1021, _mitreAttackTechnique:T1021.001, _mitreAttackTechnique:T1078, _mitreAttackTechnique:T1078.001, _mitreAttackTechnique:T1078.002, _mitreAttackTechnique:T1078.003|
## Vendors and Products
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|listMatches|
|Normalized Schema|logonType|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|user_username|


