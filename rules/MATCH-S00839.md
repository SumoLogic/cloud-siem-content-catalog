# [Rules](README.md): Azure Virtual Machine RunCommand Issued

## Description
Azure provides administrators with the ability to issue commands to Azure Virtual Machines via CLI or the Azure portal. Threat actors may use Azure privilege to run commands on virtual machines in order to further their access or move from the control plane to the compute portion of Azure.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Execution|
|Apply Risk to Entities|user_username|
|Signal Name|Azure Virtual Machine RunCommand Issued|
|Summary Expression|{{user_username}} has run a command on the Azure Virtual Machine {{device_hostname}}|
|Score/Severity|Static: 4|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0002, _mitreAttackTechnique:T1204|
## Vendors and Products
- [Microsoft - Azure](../products/a1225af5-e778-4068-a9a2-47da93d1ff24.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|description|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|user_username|


