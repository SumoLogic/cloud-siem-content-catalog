# [Rules](README.md): Suspicious Linux Execution Chain

## Description
This alert looks for a number of search expressions that result in a suspicious Linux execution chain. Specifically, a file that is created in a users' home directory or in /tmp, followed by a chmod and file execution, as well as the process making a network connection.

## Additional Details
|Detail|Value|
|----|----|
|Type|Chain|
|Category|Execution|
|Apply Risk to Entities|user_username|
|Signal Name|Suspicious Linux Execution Chain|
|Summary Expression|A suspicious execution chain has ran by {{user_username}}|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|True|
|Tags|_mitreAttackTactic:TA0002, _mitreAttackTactic:TA0001|
## Vendors and Products
- [Linux - Sysmon for Linux](../products/b238758d-ade8-41d2-b32d-c99159e9fd74.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|action|
|Normalized Schema|changeTarget|
|Normalized Schema|matches|
|Normalized Schema|metadata_vendor|
|Normalized Schema|objectType|
|Normalized Schema|user_username|


