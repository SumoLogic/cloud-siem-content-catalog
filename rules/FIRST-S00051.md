# [Rules](README.md): First Seen Inbound Network Protocol and DstPort pair

## Description
First observed inbound network traffic IP protocol and Destination Port pair. This alert is primarily informational, providing context of First Seen remote activity inbound to services or devices, and providing a record of when said activity was first observed to add context when investigating an entity's behavior. Recommended actions if this signal is observed in an Insight is to assess the contextual relevance to the behavior observed and determine if the source or destination requires further information. Searching for the external Source IP for suspicious, malicious, and questionable activity will provide important context for ascertaining the nature of the observed behavior.

## Additional Details
|Detail|Value|
|----|----|
|Type|First Seen|
|Category|Command and Control|
|Apply Risk to Entities|srcDevice_ip, dstDevice_ip|
|Signal Name|First Seen Inbound Network IP Protocol and DstPort pair - Src IP: {{srcDevice_ip}} to Dest IP: {{dstDevice_ip}} on Port: {{dstPort}}|
|Summary Expression|First Seen Network IP Protocol and DstPort pair - Inbound from {{srcDevice_ip}} to Port {{dstPort}}|
|Retention Window|7776000000|
|Baseline Window|1209600000|
|Baseline Type|GLOBAL|
|Score/Severity|Static: 4|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTechnique:T1595, _mitreAttackTechnique:T1590, _mitreAttackTechnique:T1071, _mitreAttackTactic:TA0011, _mitreAttackTactic:TA0043|
## Vendors and Products


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|dstDevice_ip|
|Normalized Schema|dstPort|
|Normalized Schema|ipProtocol|
|Normalized Schema|objectClassification|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|srcDevice_ip_isInternal|
|Normalized Schema|srcPort|
|Normalized Schema|success|


