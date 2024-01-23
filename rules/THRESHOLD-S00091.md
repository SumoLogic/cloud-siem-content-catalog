# [Rules](README.md): GCP Port Scan

## Description
Attackers will often perform reconnaissance against customer environments to better understand resources on the network. This rule looks for a single source IP scanning for different ports across the same destination.

## Additional Details
|Detail|Value|
|----|----|
|Type|Threshold|
|Category|Discovery|
|Apply Risk to Entities|srcDevice_ip|
|Signal Name|GCP Port Scan|
|Summary Expression|Port scan detected from {{srcDevice_ip}}|
|Threshold Count|25|
|Threshold Window|5m|
|Score/Severity|Static: 1|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0007, _mitreAttackTactic:TA0043, _mitreAttackTechnique:T1046, _mitreAttackTechnique:T1595, _mitreAttackTechnique:T1595.001|
## Vendors and Products
- [Google - Google Cloud Platform](../products/dcc85cfc-a698-4d09-87de-f2c723f3ad07.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|dstDevice_ip_isInternal|
|Normalized Schema|dstPort|
|Normalized Schema|listMatches|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|srcDevice_ip_isInternal|


