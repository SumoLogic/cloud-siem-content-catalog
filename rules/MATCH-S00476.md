# [Rules](README.md): Suspicious Execution of Search Indexer

## Description
From FireEye Red Team Tool Countermeasures: This IOC detects suspicious execution of searchindexer. This technique is known to be used by Cobaltstrike which inject malicious code into a newly spawned searchindexer process to evade detection.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Defense Evasion|
|Apply Risk to Entities|device_hostname, device_ip, user_username|
|Signal Name|Suspicious Execution of Search Indexer|
|Summary Expression|Suspicious command on host: {{device_hostname}}|
|Score/Severity|Static: 5|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0005, _mitreAttackTechnique:T1036, _mitreAttackTechnique:T1036.005|
## Vendors and Products
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|baseImage|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|file_path|
|Normalized Schema|parentBaseImage|
|Normalized Schema|user_username|


