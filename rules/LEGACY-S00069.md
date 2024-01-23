# [Rules](README.md): RDP Error Messages

## Description
When setting up an RDP connection, there are a number of  negotiation steps that happen.  If a connection is enrypted, not all of these can be analyzed.  Errors can indicate an operational issue or potential exploitation of a vulnerability in negotiation.

## Additional Details
|Detail|Value|
|----|----|
|Type|Match|
|Category|Execution|
|Apply Risk to Entities|device_hostname, device_ip, srcDevice_hostname, srcDevice_ip, user_username|
|Signal Name|RDP Error Messages|
|Summary Expression|Errors in RDP connection from IP: {{srcDevice_ip}} to IP: {{dstDevice_ip}}|
|Score/Severity|Static: 1|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0001, _mitreAttackTactic:TA0003, _mitreAttackTactic:TA0004, _mitreAttackTactic:TA0005, _mitreAttackTactic:TA0008, _mitreAttackTechnique:T1078, _mitreAttackTechnique:T1078.003, _mitreAttackTechnique:T1078.002, _mitreAttackTechnique:T1078.001, _mitreAttackTechnique:T1021.001, _mitreAttackTechnique:T1021, _mitreAttackTactic:TA0011, _mitreAttackTechnique:T1219|
## Vendors and Products
- [Bro - Bro](../products/37C866BF-72E1-470A-9072-EDB908F56951.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|bro_rdp_result|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|listMatches|
|Normalized Schema|srcDevice_hostname|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|user_username|


