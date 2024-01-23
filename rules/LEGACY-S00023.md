# [Rules](README.md): DCERPC - SAMR Enumeration of All Users

## Description
Microsoft provides a protocol called SAMR which stands for Security Account Manager Remote Protocol. It is designed for developers to perform (RPC) remote procedure calls for interacting the account database for both local and remote Activity Directory domains. It contains a method called SamrEnumerateUsersInDomain which return a list of users in a domain. Attackers who have network access to the domain can use this method to enumerate a list of user accounts in Active Directory. This signal looks for an RPC connection using the SAMR protocol with the method SamrEnumerateUsersInDomain signifying a request to enumerate user accounts over the network.

## Additional Details
|Detail|Value|
|----|----|
|Type|Match|
|Category|Discovery|
|Apply Risk to Entities|srcDevice_ip|
|Signal Name|DCERPC - SAMR Enumeration of All Users|
|Summary Expression|{{bro_dceRpc_operation}} undertaken from: {{srcDevice_ip}} to: {{dstDevice_ip}}|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0007, _mitreAttackTactic:TA0008, _mitreAttackTechnique:T1021, _mitreAttackTechnique:T1087, _mitreAttackTechnique:T1087.001, _mitreAttackTechnique:T1087.002, _mitreAttackTechnique:T1021.006, _mitreAttackTechnique:T1021.002|
## Vendors and Products
- [Bro - Bro](../products/37C866BF-72E1-470A-9072-EDB908F56951.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|bro_dceRpc_endpoint|
|Normalized Schema|bro_dceRpc_operation|
|Normalized Schema|srcDevice_ip|


