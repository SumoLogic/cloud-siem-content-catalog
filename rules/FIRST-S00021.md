# [Rules](README.md): First Seen Azure Virtual Machine Run Command Issued by User

## Description
A user has issued an Azure Virtual Machine run command for the first time in the baseline period.

## Additional Details
|Detail|Value|
|----|----|
|Type|First Seen|
|Category|Execution|
|Apply Risk to Entities|user_username|
|Signal Name|First Seen Azure Virtual Machine Run Command Issued by User|
|Summary Expression|Threat actors may leverage various levels of Azure Active Directory access in order to issue commands to Azure Virtual Machines via the Azure portal, resulting in potential privilege escalation avenues.|
|Retention Window|7776000000|
|Baseline Window|1209600000|
|Baseline Type|GLOBAL|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0002, _mitreAttackTechnique:T1204, _mitreAttackTechnique:T1651|
## Vendors and Products
- [Microsoft - Azure](../products/a1225af5-e778-4068-a9a2-47da93d1ff24.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|description|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|user_username|


