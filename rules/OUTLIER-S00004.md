# [Rules](README.md): Spike in Azure Firewall Deny Events from Source IP

## Description
This rule is designed to detect spikes of excessive firewall deny events within Azure for the same source IP based on a daily outliers standard deviation using a designated historic baseline. The minimum floor of firewall denies expected by default is set to 30. Customers will need to adjust the Model Sensitivity threshold (standard deviation multiplier) and Minimum Count Value of this rule to align with their environment's normal vs abnormal firewall traffic patterns.

## Additional Details
|Detail|Value|
|----|----|
|Type|Outlier|
|Category|Discovery|
|Apply Risk to Entities|srcDevice_ip|
|Signal Name|Spike in Azure Firewall Deny Events from Source IP|
|Summary Expression|Excessive count of deny Azure Firewall events identified for Source IP: {{srcDevice_ip}} based on daily historic activity|
|Retention Window|7776000000|
|Baseline Window|1296000000|
|Standard Deviation Threshold|4|
|Floor Value|30|
|Score/Severity|Static: 2|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0007, _mitreAttackTechnique:T1046|
## Vendors and Products
- [Microsoft - Azure](../products/a1225af5-e778-4068-a9a2-47da93d1ff24.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|description|
|Normalized Schema|metadata_product|
|Normalized Schema|normalizedAction|
|Normalized Schema|srcDevice_ip|


