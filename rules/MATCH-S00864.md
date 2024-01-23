# [Rules](README.md): Azure Firewall Rule Modified

## Description
The Azure Firewall may provide egress and ingress controls for a variety of Azure services, unexpected or unplanned firewall modifications should be investigated.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Defense Evasion|
|Apply Risk to Entities|user_username|
|Signal Name|Azure Firewall Rule Modified or Created|
|Summary Expression|Azure Firewall Rule Modified or Created or Created by {{user_username}}|
|Score/Severity|Static: 5|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0005, _mitreAttackTechnique:T1562.007|
## Vendors and Products
- [Microsoft - Azure](../products/a1225af5-e778-4068-a9a2-47da93d1ff24.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|description|
|Direct from Record|fields["resultType"]|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_product|
|Normalized Schema|user_username|


