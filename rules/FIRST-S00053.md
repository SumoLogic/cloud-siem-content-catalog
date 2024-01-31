# [Rules](README.md): First Seen Outbound Network Protocol and DstPort pair

## Description
First observed outbound network traffic IP protocol and Destination Port pair. This detection provides contextual information around observed outbound traffic. If this signal is observed in a suspicious context, it is recommended to investigate the host and corresponding activity on the host related to the source IP address, and the services related to the observed connection to the destination IP address.

## Additional Details
|Detail|Value|
|----|----|
|Type|First Seen|
|Category|Command and Control|
|Apply Risk to Entities|srcDevice_ip, dstDevice_ip|
|Signal Name|First Seen Outbound Network IP Protocol and DstPort pair - Source IP: {{srcDevice_ip}} to Destination Port: {{dstPort}}|
|Summary Expression|First Seen Outbound Network IP Protocol and DstPort pair observed from {{srcDevice_ip}} to Port {{dstPort}} on {{dstDevice_ip}}|
|Retention Window|2592000000|
|Baseline Window|1209600000|
|Baseline Type|GLOBAL|
|Score/Severity|Static: 1|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTechnique:T1071, _mitreAttackTechnique:T1001, _mitreAttackTactic:TA0011|
## Vendors and Products


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|dstDevice_ip|
|Normalized Schema|dstDevice_ip_isInternal|
|Normalized Schema|dstPort|
|Normalized Schema|objectClassification|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|srcDevice_ip_isInternal|
|Normalized Schema|srcPort|


