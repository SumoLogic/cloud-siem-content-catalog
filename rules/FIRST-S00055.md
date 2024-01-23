# [Rules](README.md): First Seen Denied Inbound Autonomous System (AS) Interaction

## Description
First inbound interaction observed from a Autonomous System (AS) or external network from the Internet since the baseline period. Autonmous Systems are a collection of connected Internet Protocol (IP) routing prefixes under the control of one or more network operators on behalf of a single administrative entity or domain, that presents a common and clearly defined routing policy to the Internet.  This detection identifies the first interaction with a never seen before ASN,  Investigation is recommended to gather context (protocols, requests, etc.) around the Source IP address and ASN (srcDevice_ip_asnNumber) to assess the interaction(s).

## Additional Details
|Detail|Value|
|----|----|
|Type|First Seen|
|Category|Discovery|
|Apply Risk to Entities|dstDevice_ip, srcDevice_ip|
|Signal Name|First Seen Denied Inbound Interaction with Autonomous System (AS) {{srcDevice_ip_asnOrg}}  to {{dstDevice_ip}}|
|Summary Expression|First Seen denied inbound interaction from the Autonomous System {{srcDevice_ip_asnOrg}}|
|Retention Window|7776000000|
|Baseline Window|86400000|
|Baseline Type|GLOBAL|
|Score/Severity|Static: 1|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTechnique:T1071.001, _mitreAttackTechnique:T1595, _mitreAttackTactic:TA0011, _mitreAttackTactic:TA0043|
## Vendors and Products
- [Amazon AWS - VpcFlowLogs](../products/021d1ded-1c82-4663-bf5d-d6ed5170efa3.md)
- [Microsoft - Azure](../products/a1225af5-e778-4068-a9a2-47da93d1ff24.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|dstDevice_ip|
|Normalized Schema|normalizedAction|
|Normalized Schema|objectClassification|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|srcDevice_ip_asnNumber|
|Normalized Schema|srcDevice_ip_asnOrg|
|Normalized Schema|srcDevice_ip_isInternal|


