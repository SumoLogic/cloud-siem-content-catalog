# [Rules](README.md): Multiple Azure Firewall Deny Events for IP

## Description
An Azure firewall has denied a large number of request from an IP address within a short time window.

## Additional Details
|Detail|Value|
|----|----|
|Type|Threshold|
|Category|Command and Control|
|Apply Risk to Entities|srcDevice_ip|
|Signal Name|Multiple Azure Firewall Deny Events for IP|
|Summary Expression|Multiple Azure Firewall Deny Events from {{srcDevice_ip}}|
|Threshold Count|20|
|Threshold Window|CUSTOM|
|Score/Severity|Static: 2|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0011, _mitreAttackTechnique:T1071|
## Vendors and Products
- [Microsoft - Azure](../products/a1225af5-e778-4068-a9a2-47da93d1ff24.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|description|
|Normalized Schema|metadata_product|
|Normalized Schema|normalizedAction|
|Normalized Schema|srcDevice_ip|


