# [Rules](README.md): Scheduled Task Creation with Suspicious Task Executable

## Description
Attackers may create scheduled tasks to execute commands in various scenarios. Inclusion of commonly abused or high risk Windows executables may be an indication of an attack.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Execution|
|Apply Risk to Entities|device_hostname, device_ip, user_username|
|Signal Name|Scheduled Task Creation with Suspicious Task Executable|
|Summary Expression|Scheduled task created on host: {{device_hostname}} with task content: {{fields['EventData.TaskContent']}}|
|Score/Severity|Static: 1|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0002, _mitreAttackTactic:TA0003, _mitreAttackTactic:TA0004, _mitreAttackTechnique:T1053, _mitreAttackTechnique:T1053.002, _mitreAttackTechnique:T1053.005|
## Vendors and Products
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Direct from Record|fields['EventData.TaskContent']|
|Direct from Record|fields['insertionstrings_f06']|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|user_username|


