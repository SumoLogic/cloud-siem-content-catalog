# [Rules](README.md): Amazon VPC - Network Scan

## Description
Attackers will often perform reconnaissance against customer environments to better understand resources on the network. In doing this behavior they are usually blocked by firewall rules while performing their discovery. This rule looks for a single source IP address network traffic by AWS security groups to at least 10 different destination IP addresses within a 5-minute window.

## Additional Details
|Detail|Value|
|----|----|
|Type|Threshold|
|Category|Discovery|
|Apply Risk to Entities|srcDevice_ip|
|Signal Name|Amazon VPC - Network Scan|
|Summary Expression|Potential network scan activity detected from {{srcDevice_ip}}|
|Threshold Count|25|
|Threshold Window|5m|
|Score/Severity|Static: 1|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0007, _mitreAttackTactic:TA0043, _mitreAttackTechnique:T1046, _mitreAttackTechnique:T1595, _mitreAttackTechnique:T1595.001, _mitreAttackTechnique:T1595.002|
## Vendors and Products
- [Amazon AWS - VpcFlowLogs](../products/021d1ded-1c82-4663-bf5d-d6ed5170efa3.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|dstDevice_ip_isInternal|
|Normalized Schema|dstPort|
|Normalized Schema|listMatches|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|srcDevice_ip_isInternal|


