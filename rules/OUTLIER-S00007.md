# [Rules](README.md): Spike in Windows Administrative Privileges Granted for User

## Description
Observes granting of administrative privileges in Windows environments where the number of systems accessed by a single user exceeds standard deviation of what is expected for the user based on a historic baseline. The minumum floor of unique systems expected by default is set to 1.

## Additional Details
|Detail|Value|
|----|----|
|Type|Outlier|
|Category|Privilege Escalation|
|Apply Risk to Entities|user_username|
|Signal Name|Spike in Windows Administrative Privileges Granted for User: {{user_username}}|
|Summary Expression|Outlier in distinct count of systems identified with Windows Administrative Privileges Granted for user: {{user_username}} based on hourly historic activity|
|Retention Window|7776000000|
|Baseline Window|432000000|
|Standard Deviation Threshold|2|
|Floor Value|1|
|Score/Severity|Static: 2|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0004, _mitreAttackTechnique:T1078.002|
## Vendors and Products
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|user_username|


