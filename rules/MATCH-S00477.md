# [Rules](README.md): Suspicious Use of Workflow Compiler for Payload Execution

## Description
From FireEye Red Team Tool Countermeasures: This IOC detects indicators associated with suspicious execution of Microsoft WorkFlow Compiler. This is known to be used by Cobaltstrike for lateral movement with specially crafted XLM and OXLM files.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Execution|
|Apply Risk to Entities|device_hostname, device_ip, user_username|
|Signal Name|Suspicious Use of Workflow Compiler for Payload Execution|
|Summary Expression|Parent process: {{parentBaseImage}} spawned process: {{baseImage}} on host: {{device_hostname}}|
|Score/Severity|Static: 5|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0002, _mitreAttackTactic:TA0005, _mitreAttackTechnique:T1059, _mitreAttackTechnique:T1059.003, _mitreAttackTechnique:T1127, _mitreAttackTechnique:T1127.001|
## Vendors and Products
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|commandLine|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|parentBaseImage|
|Normalized Schema|user_username|


