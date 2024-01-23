# [Rules](README.md): DCE-RPC Service Control Call

## Description
The Remote Procedure Call (RPC) protocol allows remote administrative commands to be executed.  Creating/Deleting Services , when combined with other signals can be part of an attempt to expand influence inside a network using SMB and related protocols. 

## Additional Details
|Detail|Value|
|----|----|
|Type|Match|
|Category|Lateral Movement|
|Apply Risk to Entities|srcDevice_ip, dstDevice_ip|
|Signal Name|DCE-RPC Service Control Call|
|Summary Expression|{{bro_dceRpc_operation}} undertaken from: {{srcDevice_ip}} to {{dstDevice_ip}}|
|Score/Severity|Static: 2|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0008, _mitreAttackTechnique:T1021, _mitreAttackTechnique:T1021.006, _mitreAttackTechnique:T1021.002|
## Vendors and Products
- [Bro - Bro](../products/37C866BF-72E1-470A-9072-EDB908F56951.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|bro_dceRpc_operation|
|Normalized Schema|dstDevice_ip|
|Normalized Schema|srcDevice_ip|


